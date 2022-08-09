# LaserDefender


## Learn to use

window -> package manager -> Input System

 [HideInInspector] 

### sharder
sharder Particles/Stantard Unlit
Rendering Mode => Additive

## somthing new to me

```csharp
using UnityEngine.InputSystem;

public class Player : MonoBehaviour
{
    Vector2 rawInput;

    void OnMove(InputValue value)
    {
        rawInput = value.Get<Vector2>();
    }
}
```

```csharp
Mathf.Clamp();
```
```csharp
float.MaxValue
```
```csharp
 void PlayHitEffect()
    {
        if (hitEffect != null)
        {
            ParticleSystem instance = Instantiate(hitEffect, transform.position, Quaternion.identity);
            Destroy(instance.gameObject, instance.main.duration + instance.main.startLifetime.constantMax);
        }
    }
```
```csharp
 transform.position = initialPosition + (Vector3)Random.insideUnitCircle * shakeMangitude;
```
## where u can download assets

[kenny.nl/assets/](https://www.kenney.nl/assets/)