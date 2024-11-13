# 1. Савченко Виктор

## 2. +79114828630, sawa2909@gmail.com

> 3. Получить знания от курса 

#### 4. C#, Unity2D

#### 5. Код для передвежение персонажа:
```
{
    float speed = 3f;
    float gravity = 20f;

    Vector3 direction;
    CharacterController controller;
    // Use this for initialization
    void Start()
    {
        controller = GetComponent<CharacterController>();
    }

    // Update is called once per frame
    void Update()
    {
        float x = Input.GetAxis("Horizontal");
        float z = Input.GetAxis("Vertical");

        if (controller.isGrounded)
        {
            direction = new Vector3(x, 0f, z);
            direction = transform.TransformDirection(direction) * speed;
        }
        direction.y -= gravity * Time.deltaTime;
        controller.Move(direction * Time.deltaTime);
    }
}
```
#### 6. Нет

#### 7. Среднее профессиональное: информационные системы и безопасность

#### 8. А2


