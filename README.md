# Image Reconstruction from multiple OCT Partial Images
 Optical coherence tomography (OCT) is an optical imaging method. It can be considered analogous to ultrasound imaging with greater resolution but lower penetration depth. OCT cannot penetrate the tooth fully to observe tooth decay in-between teeth, since this area cannot be accessed directly, unlike with X-rays. 
 
This project attempts to reconstruct a 3D image of a tooth from partial 2D images taken from the side of a tooth which are normally accessible. Various techniques were explored both in terms of image capture and image registration.

 

## Contents:

### Code:


* composePath.m function used to automatically compose path to load OCT image stack generated by scanner
* loadOCT.m main function used to load image stacks

preliminary.m		script used to manipulate preliminary images provided by Dr Tomlins
reload_script.m		script used to reload images into matlab
saveAsPNGstack.m	save volume to PNG stack
yStack.m		script used to manipulate y_stack images
loadRotatingOCT.m	function used to load z-stack images (modified from code kindly provided by Dr Tomlins)

Reference Images: contains images captured using other techniques used for comparison in the project
	- DiagnoCAM results.docx		contains images captured using KaVo DiagnoCAM
						(see sections 2.3.2 and 3.5.1)
	- x1ba_XMT_png.zip			contains the image captured using micro-CT as an image stack which
				  		can also be loaded using reload_script.m
						(see sections 2.3.1.1 and 3.5.2)
	- X-Ray Images of tooth X1ba.docx	x ray images of tooth
						(see sections 2.3.1 and 3.5.2)

Results: manipulated images obtained
	- 4-1-1_Results			results as described in section 4.1.1
	- 4-1-3_Results			results as described in section 4.1.3
	- 4-1-3_Results(proximal)	results as described in section 4.1.3 including proximal view
	- 4-3_Registered		results as described in section 4.3
	- 4-2_thetaStack		results as described in section 4.2
	- 4-2_thetaStack_90		results with 90 degrees angle as described in section 4.2
	- 4-2_thetaStack_120		results with 120 degrees angle as described in section 4.2
	- 4-2_thetaStack_150		results with 150 degrees angle as described in section 4.2

Unprocessed Images
	- preliminary		preliminary images used in section 4.1
	- theta_stack		theta stack used in section 4.2
	- y_stack		y stack used in section 4.3

=================================
Materials can be found at:
	https://drive.google.com/drive/folders/18xf7nIFGK93BPNGjtlPZK1dyWQtyF0BX?usp=sharing
