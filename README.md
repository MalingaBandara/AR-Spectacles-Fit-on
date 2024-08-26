
# AR-Spectacles-Fit-on

## Project Overview

AR Spectacles Fit-On is an augmented reality application developed as my final year project. The app allows users to virtually try on different spectacle frames using ARKit on iPhone devices. The primary goal is to minimize the need for physically fitting spectacle frames by offering a seamless virtual experience.

## About
AR Spects Fit-On is an app that can virtually apply spectacles frames to your face. With this app you can virtually get an image like the one you get by wearing Physical spectacles on your face. The purpose of this application is to minimize the need to select a spectacle frame using the physical fitting of the spectacle frame. This app virtually fits spectacles frames using AR technology. To do that you must have enabled ARKit on the iPhone. The ARKit feature is provided in Apple iPhone devices released after the Apple iPhone X. There is a hidden mask for face recognition, Unity software wants to use that mask to locate and adjust the point where the spectacle frames should be placed on a real face. Blender software is used to create 3D frame objects. The other parts are done by using Xcode.


## Key Features

- **AR-Based Frame Fitting**: Accurately fits virtual spectacle frames on the user's face using ARKit.
- **Unity for Face Recognition**: Utilizes Unity to adjust frame positions based on facial recognition points.
- **3D Models in Blender**: 3D spectacle frames are designed using Blender for a realistic fit.
- **Compatible Devices**: The app is designed for iPhone X and later, which support ARKit.

## Technologies Used

- **Swift and ARKit** for iOS development
- **Unity** for face recognition and frame adjustment
- **Blender** for 3D modeling of spectacle frames
- **Xcode** for development and deployment

## Project Structure and Code Explanation

1. **Face Recognition and AR Setup**:
   - ARKit is used for detecting facial landmarks and positioning the frames.
   ```swift
   func configureARSession() {
       let configuration = ARFaceTrackingConfiguration()
       arView.session.run(configuration)
   }
   ```

2. **Frame Adjustment Using Unity**:
   - Unity processes the facial data and adjusts the position of the virtual frames.
   ```csharp
   void AdjustFramePosition() {
       // Code to adjust frames based on ARKit input data
   }
   ```

3. **3D Model Integration with Blender**:
   - Blender is used to design realistic 3D spectacle models, which are imported into the app.
   ```swift
   func load3DModel() {
       // Import and render 3D models of spectacle frames
   }
   ```

## Project Output

Here are some screenshots showcasing the app's features:

<h4>01).App icon</h4>
 <img src="https://github.com/MalingaBandara/AR-Spectacles-Fit-on/blob/main/app.PNG" width="150vh" >


<h4>02). Welcome Screen</h4>
 <img src="https://github.com/MalingaBandara/AR-Spectacles-Fit-on/blob/main/welcome.PNG" width="150vh" >
 
<h4>03). Frames Trying screen </h4>
 <img src="https://github.com/MalingaBandara/AR-Spectacles-Fit-on/blob/main/t1.PNG" width="150vh" >
 <img src="https://github.com/MalingaBandara/AR-Spectacles-Fit-on/blob/main/t2.PNG" width="150vh" >

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/MalingaBandara/AR-Spectacles-Fit-on.git
   ```
2. Open the project in Xcode.
3. Run the app on an iPhone device with ARKit enabled.

## Purpose and Future Enhancements

This project was developed to explore ARKit’s potential for practical applications in retail. Future improvements could include adding more frame designs, optimizing performance, and supporting more devices.

## License

This project is licensed under the MIT License.
