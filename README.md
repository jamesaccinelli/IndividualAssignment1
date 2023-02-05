# IndividualAssignment1

Logic <br>
Diffuse lighting basis around adding colour to an object. This shader uses the built-in lambert lighting model to enhance the colouring of the object. This is done by attaching the albedo component to the colour’s rgb value. <br>

I found that Diffuse fit in well with the rest of the game’s environment, so I used it on a variety of objects. <br>

Specular lighting basis around adding a shine to an object. This shades use the built-in BlinnPhong lighting model to add a finishing polish/shininess to the object. This is done by a series of mathematical calculations. These include, adding the light direction and view direction, then normalizing it, using the dot product on the normal and light direction, as well as the normal and the normalized value we got previously. The colour of the shine is then brought together by the results of these calculations multiplied together along with other variables we create, the resulting value is assigned to the rgb value. <br>

I used specular to experiment and see how far I could push the boundaries with my shaders. <br>

Rim Lighting creates a faint glow/border of colour around the outside of an object. THis is done by setting a rim colour and rim power, the intensity of the glow/rim effect. These changes are applied via certain mathematical calculations. This includes dotting the normalized view direction and normal, then saturating it, along with multiplying the rimcolour’s rgb value with the rim value we solved for prior to the power of the rimpower/intensity mentioned earlier. <br>

Rim Lighting fit very well on parts of the towers. <br>

This standardpbr shader adds a metallic finish to objects. This is done by creating a metallic value and assigning a metallic variable to it. <br>

This shader helped give smaller edges a finished look to them. <br>

ColourGrading alters the hue and saturation of the scene to create colours and vibrance we could not create before. This is done by using a lookup table to modify the colouring. <br>


