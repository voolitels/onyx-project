#Hier hat man die Möglichkeit das Auto zu starten.

# StartEngine StopEngine #

var firstTex: Texture2D;
var secondTex: Texture2D;
var startS : AudioSource;
var stopS : AudioSource;



function Update()
{
> if(Input.GetKeyDown(KeyCode.S))
> {
> guiTexture.texture = secondTex;
> > startS.Play();

> }

> if(Input.GetKeyDown(KeyCode.A))
> {
> guiTexture.texture = firstTex;
> > stopS.Play();

> }
}



# Details #

  * eim Drück von "s" start das Auto und beim Drück von "A" halt man den motor 
