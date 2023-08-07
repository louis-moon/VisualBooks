# VisualBooks: Turning Written Books into Animated Visuals
## Introduction
VisualBooks aims to bring the textual world of books to life by turning them into animated visuals. Harnessing the power of generative AI, this project seeks to generate a series of images that, when combined, produce a gif-like representation. Imagine syncing this with an audiobook and experiencing a new form of storytelling—a blend of the traditional audio narration with AI-generated visual animations.

Originally designed for the nonprofit startup Equity A1, this repository serves as the minimum viable product (MVP) for VisualBooks.

## Features
- GPU Check: Before running any operations, the code ensures the available GPU memory is sufficient, alerting the user if there's a deficiency.
- AI Backend: Utilizes the capabilities of the VQGAN and CLIP models to generate imagery based on textual prompts.
- Customizable Prompts: Tailor your visual outputs by inputting unique textual descriptions.
- Quality Control: Control the resolution of your images by selecting between various quality options (draft, normal, better, best).
- Animated Sequences: Convert a series of images into a GIF animation, providing a visual narrative that can be synchronized with audiobook playback.
## Getting Started
### Prerequisites
It's recommended to execute this code in a Google Colab environment for compatibility and ease of GPU access.

## Setup
1. Environment Initialization (VisualBooks File):

- Start by running the Setup cell. This will:
  - Validate your available GPU memory.
  - Install necessary dependencies including PyTorch, torchvision, clipit, and more.
  - Clone essential repositories: CLIP, taming-transformers, and clipit.
  - Set up the environment for diffvg.
2. Generate Visual Imagery (animatedmovie File, Cell 2):

- Modify the prompts variable to customize the textual description for visualization.  

Example:
`prompts = "(Black-and-white stick figure image) A young boy playing with a large, happy tree. He wears a crown of leaves and acts like the king of the forest."`
- Define the quality and aspect ratio settings for your image.
- Execute the cell to get your visual output.
3. Convert Imagery to GIF (animatedmovie File, Cell 1):

- Store the images you wish to convert in a directory (e.g., 'giving_tree').
- Run the cell to process these images and obtain a GIF animation, which can be displayed directly within the notebook.
## Objective
VisualBooks redefines storytelling. By pairing AI-generated visuals with audiobooks, our aspiration is to craft an "animated movie" experience. This union offers audiences a novel, immersive storytelling medium, combining the auditory charm of narration with dynamic visual cues.
