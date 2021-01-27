# Raytracing-Utilities
A head file for wiremod Expression 2 For Raytracing

## Features

This head file includes a suite of featers for making raytracing a little less tidieous.

In the **Examples Folder** you will find several examples demoing the use of different functions and full blown raytracers using these functions!

This header include functions like:

  ###### addPass(FunctionName:string, PassScreenCordinates)
  This function allows the user to add render passes to their raytracer. This could be used to add things like bloom or denoising
    
  ###### getUvCordinates(Position:vector)
  This function allows the user to obtain uv cordinates for poisitions in the world. This can be used to map textures to surfaces.
    
  ###### lambertPDF(Direction:vector)
  This function allows the user to obtain pdfs for several different types surfaces. For more information refer to [The Render Equation File and Videos]() (Not implemented yet)
    
  ###### lambertSample(R1, R2)
  This function allows the use to obtain new bounce directions using the Lambert Diffuse PDF. This function takes two Random numbers. For more information refer to [The Render Equation File and Videos]() (Not implemented yet)
  
## Usage

To use this header file you simply include in after you directives

**Example:**

```
@name
@inputs
@outputs
@persist
@trigger

#include "Raytracing_Utilities"

if(first()){
  
  function vector render(RangerDirection:vector){
    
    # Raytracing Code here
    
    return FinalColor # Return Final Color Here
    
  }
  
}```
