# Esp32 Obtener Direccion Mac

```c++
//Variable para almacenar el chip-id
uint64_t chipid;

void setup()
{
  //Inicia el puerto serial
  Serial.begin(115200);

  //Retardo de cinco segundos
  delay(5000);

  //Obtiene el chip-id que es la direccion mac 
  chipid = ESP.getEfuseMac();

  //Imprime la direccion mac en el puerto serial
  Serial.println(chipid);
}

void loop()
{

}
```
