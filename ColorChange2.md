#Ich habe hier mit Hilfe von Unity webPage die Quelle Code bearbeitet(Farbe von jeden Objekt können getauscht sein  )
# Introduction #


using UnityEngine;
using UnityEditor;
using System.Collections;

public class ColorSi: MonoBehaviour {
> Color[.md](.md) colors = new Color[.md](.md){Color.green, Color.red, Color.blue, Color.white, Color.black , Color.cyan,
> > Color.yellow  };

> int index = 0;

> void Update(){
> > if (Input.GetKeyDown (KeyCode.W)){
> > > SetColor(colors[index++]);
> > > index = index % colors.Length;

> > }

> }

> void SetColor(Color color){
> > Renderer[.md](.md) rends = (Renderer[.md](.md))transform.root.gameObject.GetComponentsInChildren

&lt;Renderer&gt;

 ();
> > foreach (Renderer rend in rends) {
> > > foreach(Material mat in renderer.materials){
> > > > mat.color = color;

> > > }

> > }

> }
}


# Details #

Add your content here.  Format your content with:
  * **Ich habe denn diese quelle code dupliziert und mit jedem Objet verbunden . Wenn man auf Q, W, E, R kann die man die farbe tauschen.**
  * Headings, paragraphs, and lists
  * Automatic links to other wiki pages