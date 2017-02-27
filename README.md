# Project Ideas

A TODO list of all my project ideas and their status. I have epiphanies all the time and I would like to implement many of them someday. This repo holds those ideas.

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

#### Quiz application (in assoc. with R.R.)

Online Quiz authoring and administering tool

Min. Requirements:
- Quiz viewer from JSON data
- Fully responsive (all views)
- Define type of questions (free-form, multi-choice to start)

Later:
- Define more question types (image multichoice)
- Modularly build editors for different question types
- Build time or event-based quiz administration
- Define permissions
- Role creator (map of different permisisons), comes OOTB with some default roles
- User authentication (keep an internal user entity and link with other login services using OAUTH)
- Auto-save almost everywhere
