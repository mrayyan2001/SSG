### **Slide 1: البرمجة الكائنية (OOP) في 10 شرائح**

---

### **Slide 2: ما هي الـ OOP؟**

**البرمجة باستخدام "الكائنات" (Objects)**

- الكائن = **بيانات** (مثل: اللون، العمر) + **أفعال** (مثل: تشغيل، حساب).
- تجعل الكود **منظَّم** وسهل **إعادة الاستخدام**.

---

### **Slide 3: الفرق بين Class و Object**

- **Class**: وصفة لإنشاء الكائنات (مثل: وصفة لصنع سيارة).
  ```python
  class Dog:  # Class
      def bark(self):  # Method (فعل)
          print("Woof!")
  ```
- **Object**: كائن مُنشأ من الـ Class (مثل: كلب اسمه "ريكو").
  ```python
  my_dog = Dog()  # Object
  my_dog.bark()   # الناتج: "Woof!"
  ```

---

### **Slide 4: التغليف (Encapsulation)**

**إخفاء البيانات وحمايتها داخل الكائن.**

- مثال: رصيد الحساب البنكي لا يُعدَّل مباشرة، بل عبر **وظائف** مثل `get_balance()`.

---

### **Slide 5: الوراثة (Inheritance)**

**نسخ خصائص Class موجودة لإنشاء Class جديد.**

```python
class Animal:  # Parent Class
    def eat(self):
        print("Eating!")

class Cat(Animal):  # Child Class (ورثت من Animal)
    pass

my_cat = Cat()
my_cat.eat()  # الناتج: "Eating!"
```

---

### **Slide 6: تعدد الأشكال (Polymorphism)**

**نفس الاسم، أفعال مختلفة حسب الكائن.**

- مثال: دالة `move()` تعمل بشكل مختلف للـ `Car` عن الـ `Fish`.

```python
class Bird:
    def sound(self):
        print("Chirp!")

class Duck(Bird):
    def sound(self):  # Override (تعديل الوظيفة)
        print("Quack!")
```

---

### **Slide 7: التجريد (Abstraction)**

**إخفاء التعقيد، وإظهار الأساسيات فقط.**

- مثال: عند استخدام المايكرويف، تضغط زر "تشغيل" دون معرفة كيف يعمل داخلياً.
- في الكود: نحدد **ماذا** تفعل الدالة دون شرح **كيف** (مثال: `calculate_area()`).

---

### **Slide 8: لماذا نستخدم OOP؟**

1. **إعادة استخدام الكود** (بدون نسخ ولصق).
2. **صيانة أسهل** (تعديل Class واحدة بدل الكود كله).
3. **التعاون في الفريق** (كل شخص يعمل على Class منفصلة).

---

### **Slide 9: مثال واقعي**

```python
class Phone:  # Class
    def __init__(self, brand):
        self.brand = brand  # Attribute (خاصية)

    def call(self, number):  # Method
        print(f"Calling {number}...")

my_phone = Phone("Apple")  # Object
my_phone.call("123-456")   # الناتج: "Calling 123-456..."
```

---

### **Slide 10: النقاط الرئيسية**

1. الـ **Objects** تجمع بين **البيانات** و**الأفعال**.
2. الـ **Class** هي الوصفة لإنشاء الـ Objects.
3. **الأركان الأساسية**:
   - Encapsulation
   - Inheritance
   - Polymorphism
   - Abstraction

---
