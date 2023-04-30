Download Link: https://assignmentchef.com/product/solved-csc420-assignment-1
<br>
<ol>

 <li>(a)<strong> </strong>Given an <em>n</em>×<em>n </em>image <em>I</em>, and <em>m</em>×<em>m </em>filter <em>h</em>, what is the computational cost of computing <em>h </em>∗ <em>I </em>if <em>h </em>is not separable?</li>

</ol>

(b) What is the computational cost if <em>h </em>is separable?

<ol start="2">

 <li><strong> </strong>What are the steps of Canny edge detection? Please explain in detail the purpose of each step, and briefly describe how to implement each step.</li>

 <li>Explain why Laplacian of Gaussian can be used to detect edges.</li>

 <li>Please answer the following questions and submit the related code.

  <ul>

   <li>Write your own function <em>MyCorrelation </em>that implements the correlation operation. The input of the function includes: an input grayscale image <em>I</em>, a filter <em>h</em>, and a string <em>mode</em>. The function outputs the filtering results <em>J</em>. The <em>mode </em>parameter can be ’valid’, ’same’ or ’full’. The output must match what is specified by <em>mode</em>.</li>

  </ul></li>

</ol>

Please include a test sample and the results of your function in the answer.

<ul>

 <li><strong> </strong>Implement your own function <em>MyConvolution </em>that implements the convolution operation, based on the function <em>MyCorrelation</em>. The input and output is the same as <em>MyCorrelation</em>.</li>

</ul>

Please include a test sample and the results of your function in the answer.

<ul>

 <li><strong> </strong>Many camera apps provide “portrait mode”. It tends to make background objects out of focus. We can generate such effect with the knowledge in image filtering. Please select an appropriate portrait photo you like, and change it to “portrait mode”.</li>

</ul>

Please provide the type, parameters of the filter you choose, and explain the reasons for using it. Please inlcude the original image and the processed image in your answer.

(Hint: you can mannully segment out the foreground masks.) 5. Please answer the following questions and submit the related code.

<ul>

 <li><strong> </strong>Please breifly explain what is a separable filter.</li>

 <li>Please implement a function <em>isSeparableFilter</em>, which takes a filter as input and outputs a bool number indicating whether it’s seperable. If it’s seperable, print the corresponding horizontal and vertical filters.</li>

</ul>

Please show two filter samples and the results of your function in the answer.

1

<ol start="6">

 <li>Please answer the following questions and submit the related code.</li>

</ol>

<ul>

 <li>Please implement a function <em>AddRandNoise </em>to add uniformly distributed random noises on a given image. The input includes: a grayscale image <em>I</em>, the magnitude of random noises <em>m</em>. The output is the image with noises.</li>

</ul>

Use <em>AddRandNoise </em>to add noises to <em>gray.jpg</em>. Rescale the range of image to [0<em>,</em>1] and set the range of noises to [−0<em>.</em>05<em>,</em>0<em>.</em>05]. Show the image with noises in your answer.

<ul>

 <li><strong> </strong>Select appropriate linear filters to remove the noises. Please provide the type, parameters of the filter you choose, and explain the reasons for using it. Show the filtered image in your answer.</li>

 <li><strong> </strong>Please implement a function <em>AddSaltAndPepperNoise </em>to add saltand-pepper noises on a given image. The input includes: a grayscale image <em>I</em>, the density of noises <em>d</em>. The output is the image with noises.</li>

</ul>

Set the density salt-and-pepper noises to 0.05 (5% of pixels affected) and add noises to <em>gray.jpg</em>. Show the image with noise in your answer.

<ul>

 <li>Try using the filter you choose in (b) to remove the noises in (c). Does it still work now? If not, can you find a way to remove the noises? You can either implement from scratch or use existing libraries. Briefly explain the method you use and why it can work. You should demo the results in your answer.</li>

 <li><strong> </strong>Use <em>AddSaltAndPepperNoise </em>with density as 0.05, to add noises to each channel of <em>jpg</em>. Then you will get an image similar as shown in the middle of Fig. 1.</li>

</ul>

If we apply the filtering method in (d) to each channel, and then concatenate them, there will be flaws in the result. As shown in the right of Fig. 1, many noisy color blocks occurs, and the color doesn’t exist in the local region of original image. Please propose a possible solution to the flaws.

You can either implement from scratch or use existing libraries. Briefly explain the method you use and why it can work. You should demo the results in your answer.

Figure 1: From left to right: Original image, image with noises, and artifacts when applying filtering to each channel. Zoom in to have a better view.

2