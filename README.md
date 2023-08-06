# VisualBooks: Turning Written Books into Animated Visuals
## Introduction
VisualBooks aims to bring the textual world of books to life by turning them into animated visuals. Harnessing the power of generative AI, this project seeks to generate a series of images that, when combined, produce a gif-like representation. Imagine syncing this with an audiobook and experiencing a new form of storytelling—a blend of the traditional audio narration with AI-generated visual animations.

Originally designed for the nonprofit startup Equity A1, this repository serves as the minimum viable product (MVP) for VisualBooks.

## Features
- GPU Check: Before running any heavy operations, the code ensures the available GPU memory is sufficient. Alerts the user if there's a deficiency.
- AI Backend: Leverages the capabilities of the VQGAN and CLIP models to generate imagery based on textual prompts.
- Customizable Prompts: Users can input custom textual descriptions to produce corresponding visuals.
- Quality Control: Offers various quality options (draft, normal, better, best) for image generation, allowing users to balance between speed and fidelity.
## Getting Started
### Prerequisites
Ensure you're running the code in a Google Colab environment for optimal compatibility.

### Setup
1. Run the Setup cell. This will:

- Check your available GPU memory.
- Install necessary dependencies including PyTorch, torchvision, clipit, and many more.
- Clone relevant repositories: CLIP, taming-transformers, and clipit.
- Set up the environment for diffvg.
2. Run the VQGAN + CLIP cell:

- This is where the magic happens. Here, you can customize the textual prompt, choose the image quality, and decide the aspect ratio of the output image.
- Running this cell will generate the image based on your settings.
## Usage
Modify the prompts variable in the VQGAN + CLIP cell to change the textual description for the AI to visualize. For instance:

prompts = "(Black-and-white stick figure image) A young boy playing with a large, happy tree. He wears a crown of leaves and acts like the king of the forest."
## Objective
VisualBooks seeks to transform the way we experience stories. By combining these AI-generated visuals with audiobooks, our goal is to produce an "animated movie", offering users a richer and more engaging storytelling medium.
