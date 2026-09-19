# Exp02-ROLLABALL

### STEP 6 :

Create a folder in project and name as Materials [Material folder -> Create -> Material (Name: Background)

### Inspector ->Surface Inputs ->BaseMAp (Choose the color) Metallic map-> 0, Smoothness -> 0.25, Drag the Background to the plane and release the mouse

### Material folder -> Create -> Material (Name: Sphere) Inspector ->Surface Inputs ->BaseMAp (Choose the color) Metallic map-> 0,Smoothness -> 0.75,Drag the Sphere material to the ball and release the mouse

### STEP 7 : 

Hierarchy -> Player-> Inspector ->Add component-> Rigidbody
### STEP 8 : 

Create a new script -> Create a folder in project (Name: Scripts) Hierarchy -> Player -> Inspector-> AddComponent-> NewScripts-> PlayerController( Click create and Add), Copy the PlayerController and drag to Script folder, Double click the PlayerController file and type the coding

## PROGRAM :

```
Created by : JOTHI GANESH P
Reg.no : 212224240065

```

```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Code : MonoBehaviour
{
    public float Xforce =5.0f;
       public float Zforce =5.0f;
       public float Yforce =100.0f; 
    void Start()
  {
       
    }

    void Update()
    {
        float X=0.0f,Y=0.0f,Z=0.0f;
        if(Input.GetKey(KeyCode.D))
        {
            X=X-Xforce;

        }
        if(Input.GetKey(KeyCode.A))
        {
            X=X+Xforce;
        }
        if(Input.GetKey(KeyCode.D))
        {
            Z=Z-Zforce;
        }
        if(Input.GetKey(KeyCode.W))
        {
            Z=Z+Zforce;
        }
        if(Input.GetKeyDown(KeyCode.Space))
        {
            Y=Yforce;
        }
        GetComponent<Rigidbody>().AddForce(X,Y,Z);
    }
}
```

## OUTPUT :


<img width="1919" height="1084" alt="Screenshot 2026-02-03 214153" src="https://github.com/user-attachments/assets/d91f237f-d18d-4f26-8d07-40d4f8e38d12" />



## RESULT :

Thus, a 3D application for RollABall objects in unity is developed successfully.


    {
       
