# Ex5-Animator-Movement
## Aim:
To develop a animator movement for a player using unity.

## Algorithm:
## Step 1: 

Import necessary models.

## Step 2: 

 Right-click -> Create -> Animator Controller.

## Step 3: 

Open Animator window, define states (Idle, Run, Jump, etc.).

## Step 4: 

Use keyframes or Unity's Animation tools to animate transitions between states.

## Step 5: 

Drag Animator Controller to the GameObject in the Inspector.

## Program:

#### Developed by:M.PAVITHRA
#### Reg no: 212222100032

## PlayerController:
```c#
using UnityEngine;

public class movement : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;

    // Start is called once before the first execution of Update after the MonoBehaviour is created
    void Start()
    {
        animator = this.gameObject.GetComponent<Animator>();
        
    }

    // Update is called once per frame
    void Update()
    {
        InputX = Input.GetAxis("Horizontal");
        InputY = Input.GetAxis("Vertical");
        animator.SetFloat("InputX", InputX);
        animator.SetFloat("InputY", InputY);
    }
}

```
## Output:

<img width="1919" height="1095" alt="image" src="https://github.com/user-attachments/assets/efa1de63-6b16-4d9c-b590-55346f90aa51" />



## Result:

An animator movement for a player using unity is developed successfully.


