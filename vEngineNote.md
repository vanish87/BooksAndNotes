1. Singletion  
Meyers Singleton  
```c++
class Singleton {
public:
static Singleton& Instance() {
  static Singleton theSingleton;
  return theSingleton;
}
/* more (non-static) functions here */
private:
Singleton(); // ctor hidden
Singleton(Singleton const&); // copy ctor hidden
Singleton& operator=(Singleton const&); // assign op. hidden
~Singleton(); // dtor hidden
};
```
