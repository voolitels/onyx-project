Mögliche code um die Kamera in unsere Projekt zu bewegen.

= using UnityEngine;
using System.Collections;
public class Camera : MonoBehaviour
{
> public GameObject target = null;
> public bool turnArround =false;
> // Use this for initialization
> void Start () {

> }

> // Update is called once per frame
> void Update ()
> {
> > if (target != null)


> {
> > transform.LookAt(target.transform);
> > > }

> if (turnArround)
> {
> > transform.RotateAround(target.transform.position, Vector3.up, Time.deltaTime\*8);

> }

> }
} =

Add your content here.


# Details #

Add your content here.  Format your content with:
  * Text in **bold** or _italic_
  * Headings, paragraphs, and lists
  * Automatic links to other wiki pages