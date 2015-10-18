Wir haben 3 verschiedenen Camera hinzugefügt man hat die möglichkeit durch die 3 Camera das Auto zu sehen hier ist die quelleCode.

# switch Camera #



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