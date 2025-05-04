
# پیاده‌سازی Timsort به زبان پایتون

این مخزن شامل یک پیاده‌سازی ساده از الگوریتم Timsort به زبان پایتون است.
Timsort یک الگوریتم مرتب‌سازی هیبریدی است که ترکیبی از merge sort و insertion sort می‌باشد.

---

## بخش ۱: معرفی Timsort

الگوریتم Timsort توسط Tim Peters در سال ۲۰۰۲ برای زبان Python طراحی شد.
این الگوریتم در حال حاضر مرتب‌سازی پیش‌فرض در Python (توابع sorted و list.sort) و همچنین Java (برای آرایه‌های غیرپریمیتیو) است.

ویژگی‌ها:

* بهترین حالت زمانی: O(n) روی داده‌های تقریباً مرتب
* میانگین و بدترین حالت زمانی: O(n log n)
* پایدار (ترتیب المان‌های مساوی حفظ می‌شود)
* بهینه‌شده برای داده‌های واقعی با تشخیص زیرآرایه‌های مرتب (run)

---

## بخش ۲: فایل‌ها و توضیحات کلی

* timsort.py: فایل پایتون شامل پیاده‌سازی Timsort
* README.md: این فایل توضیحات

روش کلی کار الگوریتم:

1. شناسایی runها (زیرآرایه‌های مرتب)
2. مرتب‌سازی runهای کوچک با insertion sort
3. ادغام runها با merge sort

---

## بخش ۳: نحوه اجرا و منابع

نحوه اجرا:

```
python timsort.py
```

نمونه کد در فایل:

```
arr = [5, 21, 7, 23, 19, 10, 1, 3, 2]
print("قبل:", arr)
timsort(arr)
print("بعد:", arr)
```

منابع:

* ویکی‌پدیا: Timsort → [https://fa.wikipedia.org/wiki/Timsort](https://fa.wikipedia.org/wiki/Timsort)
* سورس کد پایتون → [https://github.com/python/cpython/blob/main/Objects/listsort.txt](https://github.com/python/cpython/blob/main/Objects/listsort.txt)

---

