wie den Überschrift sagt, es geht um den Menu an anfang des Projektes



using UnityEngine;


public class clickPassIntro : MonoBehaviour
{
> void OnGUI()
> {
> > const int buttonWidth = 100;
> > const int buttonHeight = 60;



> Rect buttonRect = new Rect(
> > Screen.width / 2 - (buttonWidth / 2),
> > (2 **Screen.height / 3) - (buttonHeight / 2),
> > buttonWidth,
> > buttonHeight
> > );**



> if (GUI.Button (buttonRect, "Adventador"))
> {

> Application.LoadLevel ("Adventador");
> }

> }
}


Add your content here.  Format your content with:
  * Text in **bold** or _italic_
  * Headings, paragraphs, and lists
  * Automatic links to other wiki pages