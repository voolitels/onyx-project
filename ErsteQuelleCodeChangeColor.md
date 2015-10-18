# Erste Versucht Auto Body´s color ohne details(Inhalt des Autos).

# In Unity gemacht #

using UnityEngine;
using UnityEditor;


public class ColorS : MonoBehaviour
{

> void Update()
> {
> > if (Input.GetKeyDown (KeyCode.Q))
> > {
> > > gameObject.renderer.material.color = Color.red;

> > }


> if (Input.GetKeyDown (KeyCode.W))
> {
> > gameObject.renderer.material.color = Color.white;

> }

> if (Input.GetKeyDown (KeyCode.E))
> {
> > gameObject.renderer.material.color = Color.blue;

> }

> if (Input.GetKeyDown (KeyCode.R))
> {
> > gameObject.renderer.material.color = Color.black;

> }

> if (Input.GetKeyDown (KeyCode.T))
> {
> > gameObject.renderer.material.color = Color.cyan;

> }

> if (Input.GetKeyDown (KeyCode.Z))
> {
> > gameObject.renderer.material.color = Color.yellow;

> }

> }



}


# Details #

Add your content here.  Format your content with:
  * **Der QuelleCode wird bearbeiten damit man auf einem Knopf Drucken kann um die Farbe zu tauschen**
  * Headings, paragraphs, and lists
  * Automatic links to other wiki pages