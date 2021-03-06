# Project Ideas

A TODO list of all my project ideas and their status. I have epiphanies all the time and I would like to implement some of them someday. This repo holds those ideas.

## Ideas
#### Animated Meme Generator

Generate embedable code for animated memes

Status: Not started

Min. Requirements:
- No DB or hosting, meme encoded as URL hash
- Editor for creating memes (image and text placement, animation templates with customization for each element)

Good to have:
- DB for meme hashes
- Top memes list (can I track where embed codes are used elsewhere?)

----

#### Image gallery based on Electron:

Cross-platform image viewer (emphasis on viewer and not editor).

Min. Requirements:
- Recursive folder browsing
- Responsive design
- Metadata display
- Automatic thumbnail caching
- __Web based image viewer spinoff__ (keep viewer code separate to use on websites)

Later:
- Completely file-based (a.k.a easily portable) tag database
- OpenCV for similar image search
- Clustering based on location, timestamp, image similarity (useful to group burst shots from cameras)
  - Ability to create collages and GIFs from images
- Panorama and PhotoSphere viewer (auto-detect panorama based on aspect ratio, possible autodetection of spheres based on image features or metadata for Google PhotoSpheres)
- Smart thumbmails (use OpenCV for area of interest detection)
- Auto-tagging based on image feature databases (use online feature DBs or cache them offline)

----

#### Quiz application (in assoc. with R.R.)

Online Quiz authoring and administering tool

Min. Requirements:
- User DB
  - Registration model with email (oauth later)
  - After login, can create/edit/delete quizes
- Define type of questions (free-form, multi-choice to start)
- Quiz Creator
  - Add diff. type of questions to an editable list
  - Option to "Publish" -> activates a permalink which is accessible publicly
  - Responsive layout (not a priority, set min-width if needed)
- Quiz viewer from JSON data
  - Just load JSON data and display different question types
  - Responsive layout (mandatory)

Later:
- Define more question types (image multichoice)
- Modularly build editors for different question types
- Time or event-based quiz administration
- Define permissions
- Role creator (map of different permisisons), comes OOTB with some default roles
- User OAUTH implementation
- Auto-save almost everywhere

----

Android geofencing based on WiFi/Bluetooth signal strength
- Close range fences like rooms without using GPS
- Similar projects exist (like https://altbeacon.github.io/android-beacon-library/index.html, I think), should look into those more and see if I can use any
- Main idea is to check viability of checking range using just WiFi/Bluetooth signal strength
- Workflow goes something like this: Place beacons and perform one-time calibration (stand in corners of room, or move along corners of room).
- Primary/moptivating usecase: keel my phone unlocked when I am home (options I know of currently are GPS-based geo-fencing or Google's on-body detection, both of which are not exactly what I want).

----

Anaglyph photo maker app

- Camera app which uses gyroscope information to guide users to take perfect pictures needed for anaglyph
- Build anaglyph
- Maybe use gyro readings to infer homography of one pic to the other and adjust it to ideal perspectives to simulate vision from 2 eyes

ALTERNATIVELY:

- Use CV to detect very similar images
- Develop an algorithm to see if similar images are good fit for an anaglyph picture (eg. detect if subjects haven't moved but perspective changed)
- Once good candidates are identified, develop algorithm to find focal point and build anaglyph image
- Typically, distance between cameras (or eyes) should be 1/30 or 1/50 of focal distance (distance from camera to focal point)

This could be a feature in the CV-assisted gallery application project

----
