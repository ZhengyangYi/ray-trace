# Zhengyang Yi ray-tracer

# What I implemented
I implemented a raytracer to rendering the samples images to the new ppm file. This is a sample ball pattern images that I have rendered.
<img width="600" alt="截屏2022-09-13 下午10 51 07" src="https://user-images.githubusercontent.com/69991827/190308013-07ec31fc-bd6b-4a9d-b483-dbf0a71d2360.png">

# The problem I encountered
The first problem I encountered was that the screen was all black and nothing was displayed, and later I found out that it was because I forgot to return the value of the pixel point normal when doing the intersection of the triangles, and successfully solved it. The second problem is that there are some shadow calculation bugs, and there is a lot of noise on the screen. I guess it is because when checking whether there is a shadow, I set the t0 of the intersect function to 0, which makes the system unable to judge here. There is no shadow, so I set t0 to a small number but not equal to 0, and it successfully solved the problem. The last question is also about the shadow, the shadow at the bottom of the object is not showing, but unfortunately, I didn't have a chance to successfully solve this problem, I think this is a function that I need to fix in the future.

<img width="400" alt="截屏2022-09-13 下午11 30 23" src="https://user-images.githubusercontent.com/69991827/190308096-c75df4d8-d90c-420f-aa94-241bf09bc5d2.png">
<img width="400" alt="截屏2022-09-13 下午10 29 28" src="https://user-images.githubusercontent.com/69991827/190308252-e61374d5-8f39-4aca-a4f4-37a4ee1c1dea.png">

# What I learned
For me, I have learned a lot of new knowledge in this subject. I am relatively lacking in programming proficiency. I have also learned the basics of programming syntax before, but I have not learned to use programming language knowledge to make something. In fact, this is my first big project, the first time to use programming to solve certain problems, which has had a huge impact on me. Moreover, the programming language I used before was java, and I also spent some time learning how to convert from java to c++, and learned many features of c++ such as pointers. But actually I think mathematics is the biggest challenge for me, because I haven't learned linear algebra before, so I spent some time learning vector calculation, and writing a structure in code to help my calculation, without Use other math libraries and just want to make new knowledge handy. In this course I learned a lot that refreshed my perception, I learned how things I normally see on a computer screen are implemented with code and graphics knowledge, which is amazing. Phong Shading, Intercections, I can't describe how excited I was when I used this knowledge to write my first ray tracer. In addition to the usual lectures, I also learned new graphics knowledge outside of class, such as texture mapping, projection, and transformation, sampling, rasterization, and noise reduction. Although I already have a basic understanding of this knowledge, the biggest challenge for me is actually to implement these functions in code, which is what I need to work on in the future.

# Future expection
I plan to use matrix to make a  transformation function, the acceleration of raytracing, refractions, and trying to figure out a way to lower the noises appear in the rendered images in the future.
