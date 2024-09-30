![image](https://github.com/user-attachments/assets/e7e0a387-b756-4595-8a85-30b17980fc09)

# Tripo_HOU: Tripo3D Integration for Houdini

Tripo_HOU is a custom Houdini node that integrates Tripo3D's AI-powered 3D model generation capabilities directly into your Houdini workflow. This node allows you to generate 3D models from text prompts or images using Tripo3D's API.

## Video Demonstration

Check out this video demonstration of Tripo_HOU in action:
[Watch on YouTube](https://www.youtube.com/watch?v=F9vX2ulNKSs)

## Features

- Generate 3D models from text prompts (Text to Model)
- Generate 3D models from images (Image to Model)
- Automatic download and import of generated models into Houdini
- Texture extraction and shader setup

## Requirements

- Houdini 19.0 or later
- Python 3.7+
- `requests` library (usually comes pre-installed with Houdini)
- Active internet connection
- Tripo3D API key

## Installation

1. Copy the `sop_Dragoy.main.tripo_hou.1.1.hda` file to your Houdini user otls directory. 
   For example, on Windows, this might be:
   `C:\Users\YourUsername\Documents\houdini20.5\otls`

   Replace `YourUsername` with your actual Windows username.

2. Restart Houdini or refresh the OTL list to make the new node available.

## Getting Started

1. Obtain a Tripo3D API key:
   - Visit [https://platform.tripo3d.ai/api-keys/](https://platform.tripo3d.ai/api-keys/)
   - Sign up or log in to your Tripo3D account
   - Generate a new API key

2. In Houdini, create a new "Tripo Hou" node in your scene. You can find it in the node creation menu under the name "Tripo Hou".

3. Set up the node parameters:
   - Enter your Tripo3D API key in the "API Key" field
   - Specify a download folder for the generated models
   - Choose the generation type (Text to Model or Image to Model)
   - For Text to Model: Enter your text prompt
   - For Image to Model: Specify the path to your input image
   - Select the model version: We recommend using version 2.0 for the best quality results

4. Click the "Generate" button to start the model generation process.

5. Wait for the process to complete. The generated model will be automatically imported into your Houdini scene with materials applied.

## Usage Tips

- Ensure your API key is kept secret and not shared publicly.
- For best results, use clear and descriptive text prompts or high-quality input images.
- The generation process may take a few minutes, depending on the complexity of the request and server load.
- You can enable logging to get more detailed information about the generation process.

## Troubleshooting

- If you encounter any errors, check the Houdini console for error messages.
- Ensure you have an active internet connection.
- Verify that your API key is correct and has not expired.
- If problems persist, you can refer to the [Tripo3D documentation](https://platform.tripo3d.ai/docs/introduction/) for more information.

## Support

For additional help or to report issues, please open an issue on the [GitHub repository](https://github.com/Dragoy/Tripo_HOU/issues).

## License

This tool is provided as-is, without any guarantees or warranty. Users are responsible for complying with Tripo3D's terms of service and API usage policies.
