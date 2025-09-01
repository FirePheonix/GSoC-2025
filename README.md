# Google Summer of Code 2025
# Sugar Labs
<p align="center">
<img src="https://github.com/user-attachments/assets/8d30793e-af8c-4ea3-af39-914392df416e" height="300px">
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</p>

## Contributor Information  

- **Name:** Shubham Singh
- **Email:** [shubhsoch@gmail.com](mailto:shubhsoch@gmail.com)  
- **GitHub:** [FirePheonix](https://github.com/FirePheonix)
- **Organization:** [Sugar Labs](https://www.sugarlabs.org/)  
- **Project Statement Repository:** [Color Sensor for Music Blocks for photos and real-time videos](https://github.com/sugarlabs/musicblocks/issues/4537)
- **Mentors:** [Walter Bender](https://github.com/walterbender), [Devin Ulibarri](https://github.com/pikurasa)
---

## Description

The goal of the project is to develop extended functionality to our existing tools of turtle/mouse glyph movement and limited color detection to sense color from uploaded images, as well as the real-time feed from a webcam. Upon successful implementation, the turtle/mouse glyph will be able to detect the color of pixels underneath it, regardless of whether those pixels were drawn by the turtle/mouse itself, part of an uploaded image stamped to the canvas, or part of a live webcam video feed into Music Blocks. One test of success is to run our Lego music notation for the blind project with a live feed. The result should be able to playback and record the abstract brick notation based on its contrasting colors.

## Background

Music Blocks has a feature to detect the color of pixels generated from drawing within the program, but it cannot detect the color of pixels from images that are either uploaded or from a webcam. By adding a feature to detect color from both uploaded images and a live webcam stream, users would be able to implement Lego music notation for the blind and similarly interactive programs.

## Goals

The main objectives of this project were to enhance the project management and learning experience in Music Blocks and Turtle Blocks by introducing a Git-based backend. Specifically, the project aimed to:

- **Replace the Planet system:** Improve the existing project storage system to support version control and better project management.
- **Enable Project Commits and Edits:** Allow students to create, save, and update their own projects, with a record of all changes.
- **Support Forking of Projects:** Let students explore and build upon other users’ projects, fostering collaboration and peer learning.
- **Provide Project History Navigation:** Enable students to view the complete history of a project, reflecting on how it has evolved over time.
- **Allow Project Downloads:** Give students the option to download their projects for offline use or portfolio creation.


The main objectives of this project were to extend the functionality of Music Blocks by enhancing its ability to detect colors not only from drawings generated within the program but also from external sources such as uploaded images and live webcam streams. Specifically, the project aimed to:

- **Expand Color Detection Capabilities:** Extend existing pixel color detection beyond turtle-drawn graphics to include uploaded images and real-time webcam feeds.
- **Support Lego Music Notation for the Blind:** Facilitate the implementation of interactive programs such as Lego music notation, where color detection plays a crucial role in accessibility and learning.
- **Enable Real-Time Interactive Feedback:** Provide immediate color-based responses from webcam streams, allowing users to create dynamic and adaptive music experiences.
- **Record and Playback Abstract Brick Notation:** Allow the system to capture, record, and replay music generated through color contrasts, creating a bridge between visual patterns and auditory output.
- **Integrate Seamlessly:** Ensure all features work smoothly within Music Blocks, maintaining an intuitive educational experience.

## Demonstration

To showcase the features of the LegoBricks musical notation Widget, please refer to the below video:

[![Watch the Demo]](https://youtu.be/jxy6Qy0iigI?feature=shared))

## Technical Implementation

# LEGO Color-to-Music Detection System for Music Blocks

An innovative system that converts LEGO block colors into musical notes through image processing and real-time webcam detection, enabling interactive music composition and automated music notation reading.

## Phase 1: Core Development (Weeks 1–6)

### Week 1: Basic UI & Image Upload System
**Goal:** Implement UI components and support image uploads.
* Develop file input for image uploads
* Add a canvas element for color processing
* Implement a basic tooltip for real-time color detection
* Ensure smooth user interaction and error handling

**Deliverable:** Functional UI with image upload support.

### Week 2-3: Color Detection & Mapping to Musical Notes
**Goal:** Extract pixel colors and map them to musical notes.
* Implement color extraction from images using getImageData()
* Convert RGB values to HSL for accurate color recognition
* Map detected colors to musical notes based on predefined rules
* Adjust saturation and contrast for better accuracy

**Deliverable:** A working prototype that converts image colors to musical notes.

### Week 4-6: Live Webcam Integration and Shadow Handling
**Goal:** Enable real-time color detection via a webcam while minimizing shadow interference.
* Integrate getUserMedia() for live webcam feed
* Process real-time video frames on the canvas
* Implement dynamic color detection from webcam input
* Develop techniques to minimize shadow interference, such as adaptive brightness and contrast adjustments
* Allow users to move objects to generate sounds interactively

**Deliverable:** A stable webcam feed that dynamically generates music based on object colors with minimal shadow interference.

## Phase 2: Enhancements & Optimization (Weeks 7–12)

### Week 7-9: Implementing the Moving Mouse for Automated Scanning
**Goal:** Automate music notation reading using a moving mouse.
* Implement a scanning algorithm that moves across the image
* Detect block lengths based on X-start and X-end positions
* Adjust Y-position to determine pitch dynamically
* Store detected notes in a data structure (stack/array) for sequential playback
* Ensure that scanning is optimized for performance

**Deliverable:** An automated scanning system that reads colors and translates them into music notation.

### Week 10-11: Sound Processing & Fine-Tuning
**Goal:** Improve sound quality, eliminate unwanted noise, and refine transitions.
* Integrate Audacity to enhance audio clarity
* Implement smooth transitions between notes
* Allow users to adjust tempo and playback speed
* Optimize real-time processing for efficiency
* Implement noise reduction strategies to avoid false note detection from minor color variations

**Deliverable:** A refined sound processing system with customizable playback options.

### Week 12: User Testing, Bug Fixes, and Documentation
**Goal:** Ensure stability and prepare the project for submission.
* Conduct user testing and gather feedback
* Identify and fix bugs in color detection, sound mapping, and UI
* Ensure cross-device compatibility (mobile, tablet, desktop)
* Write detailed documentation, including setup guides and API details
* Create tutorials or demo videos for new users
* Submit the final version to the GSoC repository

**Final Deliverable:** A fully functional and documented color-to-music system for Music Blocks.

This structured plan ensures that simpler tasks are completed quickly, while more complex features such as webcam shadow handling, moving mouse scanning, and sound optimization receive adequate development time.
## Project Timeline

| Week | Dates           | Milestones & Achievements | Blog / Report Link |
|------|----------------|---------------------------|------------------|
| Week 1 | 2025-06-01 – 2025-06-07 | Creating UIs and visuals for addition of Lego Bricks. | [Week 1](https://www.sugarlabs.org/news/all/2025-06-07-gsoc-25-FirePheonix-week01) |
| Week 2 | 2025-06-08 – 2025-06-14 | Adding the entire prototyped interface ON TO the msuci blocks. | [Week 2](https://www.sugarlabs.org/news/all/2025-06-14-gsoc-25-firepheonix-week02) |
| Week 3 | 2025-06-15 – 2025-06-21 | Mapped Music from Synthutils to LegoBricks. Completed LegoBricks Widget UIs. | [Week 3](https://www.sugarlabs.org/news/all/2025-06-25-gsoc-25-firepheonix-week03) |
| Week 4 | 2025-06-22 – 2025-06-28 | Pivoted from Point Scanner to Line Scanner, got some real results. | [Week 4](https://www.sugarlabs.org/news/all/2025-07-01-gsoc-25-firepheonix-week04) |
| Week 5 | 2025-06-29 – 2025-07-05 | Building and testing out the image to video player. | [Week 5](https://www.sugarlabs.org/news/all/2025-07-05-gsoc-25-firepheonix-week05) |
| Week 6 | 2025-07-06 – 2025-07-12 | Music Player + Mid Term Evaluation. | [Week 6](https://www.sugarlabs.org/news/all/2025-07-13-gsoc-25-firepheonix-week06) |
| Week 7 | 2025-07-13 – 2025-07-20 | Method to simplify musical notes and export as action blocks. | [Week 7](https://www.sugarlabs.org/news/all/2025-07-21-gsoc-25-firepheonix-week07) |
| Week 8 | 2025-07-21 – 2025-07-27 | Added method to identify blocks as phrase maker objects. | [Week 8](https://www.sugarlabs.org/news/all/2025-07-28-gsoc-25-firepheonix-week08) |
| Week 9 | 2025-07-28 – 2025-08-03 | Successfully implemented action block export functionality. | [Week 9](#) |
| Week 10 | 2025-08-04 – 2025-08-10 | Fixed some Image overflow and accuracy issues in scanning. | [Week 10](#) |
| Week 11 | 2025-08-11 – 2025-08-17 | Added SVGs, more instruments, auto arrange method in LegoBricks widget. | [Week 11](#) |
| Week 12 | 2025-08-18 – 2025-08-24 | Feedback incorporation, final polishing. | [Week 12](#) |

## Project Resources & Code

- **Pull Requests with Code:**   
  1)  [GitHub Repo](https://github.com/sugarlabs/musicblocks/pull/4743)
  2)  [GitHub Repo](https://github.com/sugarlabs/musicblocks/pull/4755)

- **README:** Documentation for Widget.  
  [README](https://github.com/sugarlabs/musicblocks/commit/8f113a329e5bad50df2ed26b50d937259ad90735#diff-b335630551682c19a781afebcf4d07bf978fb1f8ac04c6bf87428ed5106870f5)

- **Demo Video:** Video demonstration of the Git backend features, including commits, forks, and history navigation.  
  [Watch Demo](https://youtu.be/jxy6Qy0iigI?feature=shared)


## Future Scope (Post-GSoC)
* Expand to gesture-based interactions for composing music
* Implement AI-based pattern recognition for complex melodies
* Enable multi-user collaboration in real-time music generation

### Acknowledgments

I would like to extend my heartfelt thanks to:

- **Walter Bender & Devin Ulibarri:** For their continuous mentorship, guidance, and insightful feedback throughout the project.  
- **Sugar Labs Community:** For their support, discussions, and encouragement that helped shape the project. 

Their support was invaluable in making the Color Sensor for Music Blocks a successful and educational experience.
Overall, Google summer of Code 2025 was a great learning experience for me. Was an immense pleasure.
