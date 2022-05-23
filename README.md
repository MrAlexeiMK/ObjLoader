# ObjLoader
 C# library for loading and working with .obj models (extracted from <b><a href="https://github.com/MrAlexeiMK/StereoStructure">StereoStructure</a></b>)  
 
 ```
 string path = "/path/to/obj/file.obj"
 Model model = new Model();
 model.Load(path); //load .obj model
 
 model.ApplyOperator(new Matrix(OperatorType.ROTATION_3D_X)); //apply rotation operator around axis X
 model.Save(path); //save to same file
 
 //After model processing you can display it in HelixToolkit Framework in C# WPF
 ObjReader objReader = new ObjReader();
 model3d.Content = objReader.Read(path);
 ```
