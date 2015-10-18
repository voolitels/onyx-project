# Kamera code für das Gesamte Projekt #


Add your content here.
using UnityEngine;
using System.Collections;

public class CameraZ1 : MonoBehaviour
{
> public bool turnArround= false;
> public GameObject target = null;

> // Use this for initialization
> void Start () {

> }

> // Update is called once per frame
> void Update ()
> {
> > if (target != null)
> > {
> > > transform.LookAt(target.transform);

> > }



> if (turnArround)
> {
> > transform.RotateAround(target.transform.position, Vector3.up, Time.deltaTime\*8);

> }
> }
}












using System.Collections;



public class CameraZ : MonoBehaviour
{
> public float distance;
> private float sensitivityDistance = -7.5f;
> private float damping = 1.5f;

> private Vector3 xdistance;
> private float moveSpeed = 0.5f ;
> public GameObject target = null;


> void Start ()
> {
> > distance = 55f;
> > distance = transform.localPosition.x;

> }
> void Update ()
> {

> if (target != null)
> {
> > transform.LookAt(target.transform);

> }



> if (Input.GetMouseButton(0))
> {

> transform.Translate(Vector3.right **-Input.GetAxis("Mouse X")** moveSpeed);
> transform.Translate(transform.right **-Input.GetAxis("Mouse ")** moveSpeed, Space.World);
> }



> }

}





using UnityEngine;
using System.Collections;

public class CameraIn : MonoBehaviour
{

> public float distance;
> private float sensitivityDistance = -7.5f;
> private float damping = 1.5f;
> private float min = -100;
> private float max = -2;
> private Vector3 xdistance;
> private float moveSpeed = 0.5f ;
> float timer = 0;
> > float direction = 0.2f;



> void Start ()
> {
> > distance = 55f;
> > distance = transform.localPosition.x;

> }
> void Update ()
> {




> if (Input.GetMouseButton(0))
> {
> > transform.Rotate(Vector3.right **-Input.GetAxis("Mouse Y")** moveSpeed);



> direction **= -1;
> > transform.Rotate (new Vector3 (0, -1** direction, 0));



> }

> if (timer % 100 == 0)
> direction **= -1;
> transform.Rotate (new Vector3 (0, 1** direction, 0));
> timer++;
> }


}


> using UnityEngine;
using System.Collections;

public class Switch : MonoBehaviour {

> public Camera camera1;
> public Camera camera2;
> public Camera camera3;


> void Start () {
> > camera1.enabled = true;
> > camera2.enabled = false;
> > camera3.enabled = false;

> }

> void Update () {
> > if (Input.GetKeyDown(KeyCode.D))
> > {
> > > camera1.enabled = false;
> > > camera2.enabled = true;
> > > camera3.enabled = false;

> > }
> > if (Input.GetKeyDown(KeyCode.F))
> > {
> > > camera1.enabled = true;
> > > camera2.enabled = false;
> > > camera3.enabled = false;

> > }


> if (Input.GetKeyDown(KeyCode.G))
> {
> > camera1.enabled = true;
> > camera2.enabled = false;
> > camera3.enabled = true;

> }
> }
}




# Details #

Add your content here.  Format your content with:
  * Text in **bold** or _italic_
  * Headings, paragraphs, and lists
  * Automatic links to other wiki pages