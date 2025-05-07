# 2D-to-3D-Image_Convertor
1. Set up Virtual Environment:

First, install virtualenv if you don't have it installed already:
pip install virtualenv
Create a virtual environment:
python -m venv venv
Activate the virtual environment:
.\venv\Scripts\activate

2. Run the following command to install all required libraries:
pip install -r requirements.txt
Prepare Input:

3. Put your desired 2D image (e.g., cat.jpg) in the inputs/ folder. The image should be clear and contain only the object you want to convert into a 3D model.

4. Run the Script:

You can run the script in any Python environment or Jupyter notebook.

The script will ask for an input type — either image or text.

If you choose image, the script will:

Perform background removal using the rembg library.

Generate a 3D point cloud using Point-E.

Apply Poisson surface reconstruction to the point cloud and generate the 3D mesh.

Save the model in .obj and .stl formats.

5. Check Outputs:

After the script runs, check the outputs/ folder for the following:

Point Cloud: outputs/text_point_cloud.ply

OBJ Mesh: outputs/text_mesh.obj

STL Mesh: outputs/text_mesh.stl

# Libraries Used
numpy: Used for numerical operations in the project.

matplotlib: Used for plotting and visualizations.

opencv-python: Used for image preprocessing and handling.

Pillow: Used for image processing and background removal.

trimesh: Used for loading and visualizing 3D meshes.

pyrender: Used for 3D rendering of models.

rembg: Used for removing the background from images.

open3d: Used for point cloud and mesh processing.

torch: Used for running the Point-E model.

scikit-image: Used for image-related operations.
