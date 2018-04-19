# Gender
Quickly determine the gender of a face. Trained on hundreds of thousands of IMDB images."

**Possible Use Cases**
  * Adding gender classification to a face detection system
  * Targeted messaging to your users based on their gender/interests
    * Especially useful if you do not ask what a users gender is during registration
  * Categorizing profiles from social networks by gender


## Input Scheme
The input should contain a base64 encoded image of a face. 
``` json
{
  "image": "BASE_64_ENCODED_IMAGE"
}
```

## Output Scheme
The output will map each input text to a score. Positive receive positive scores while negative texts receive negative 
scores. 
 
``` json
{
  "woman": 0.91,
  "man": 0.09
}
```


## Training
The model was trained by the [B-IT-BOTS robotics team][1] on over 500,000 IMDB images. 


[1]: https://mas-group.inf.h-brs.de/?page_id=622