# **Building & Hosting a Web Page              بناء واستضافة صفحة ويب**


**Phase 1: Writing Code Locally & The Asset**
 **المرحلة 1: كتابة الكود محلياً ومعضلة مسارات الصور**

**1. Writing the HTML Code** 
 **كتابة كود الـ HTML**

We started by writing a simple structure in **Notepad** (or any text editor) containing a heading, a paragraph, and an image tag (`<img>`).


بدأنا بكتابة هيكل بسيط لصفحة الويب على برنامج **Notepad** (المفكرة)، يحتوي على عنوان رئيسي، فقرة تعريفية، ووسم الصورة (`<img>`).


![img alt](https://github.com/taleensami001-lgtm/From-Notepad-to-the-World-Building-Hosting-a-Web-Page/blob/401fc33dce88bb44ca4637560d0025d52f3db9ad/Screenshot%202026-07-14%20164341.png)


![img alt](https://github.com/taleensami001-lgtm/From-Notepad-to-the-World-Building-Hosting-a-Web-Page/blob/22f3d32e50a68c0f5c8efe288c37dd588e4d332b/Screenshot%202026-07-14%20164455.png)




```
<!DOCTYPE TYPE html>
<html>
<head>
    <title>Personal Page</title>
</head>
<body>
    <h1>Taleen sami alharbi</h1>
    <p>Hi my name is Taleen, I am 20 yo, I like Coffee :D</p>
    <img src="silly-cat.png" alt="meow" width="200" height="300">
</body>
</html>

```

 **2. Saving the File Locally** 
 **حفظ الملف محلياً**

When saving the file, we must set "Save as type" to **All Files** and name it `Taleen.html`.


عند حفظ الملف، يجب تغيير نوع الحفظ إلى **All Files** وتسميته باسم `Taleen.html` ليعمل كصفحة ويب.

![img alt](https://github.com/taleensami001-lgtm/From-Notepad-to-the-World-Building-Hosting-a-Web-Page/blob/401fc33dce88bb44ca4637560d0025d52f3db9ad/Screenshot%202026-07-14%20164419.png)

**The Golden Rule / القاعدة الذهبية:**
For relative image paths (like `src="silly-cat.png"`) to work locally, the image file and the HTML file **must be saved in the exact same folder** on your computer.


 لكي تعمل مسارات الصور النسبية محلياً، **يجب** حفظ ملف الصورة وملف الـ (اتش تي ام ال) في نفس المجلد تماماً على جهازكِ.


![img alt](https://github.com/taleensami001-lgtm/From-Notepad-to-the-World-Building-Hosting-a-Web-Page/blob/22f3d32e50a68c0f5c8efe288c37dd588e4d332b/Screenshot%202026-07-14%20164512.png)


**Phase 2: Why Sandbox Editors (W3Schools) "Break" Images**     
**المرحلة 2: لماذا "تخرب" الصور في محررات الويب**

When testing the same code on W3Schools Online Editor, the text loads but the image breaks, displaying only the `alt` text.


عند تجربة الكود نفسه على محرر W3Schools الإلكتروني، تظهر النصوص لكن الصورة تنكسر ويظهر النص البديل `alt` فقط.

### **The Explanation / التفسير البرمجي:**

W3Schools runs on a remote server. When it reads `src="silly-cat.png"`, it searches for that file on *its own online servers*, not on your computer. Since the image is only on your hard drive, the browser cannot find it.


يعمل موقع W3Schools على خادم بعيد. عندما يقرأ الكود `src="silly-cat.png"`، يبحث عن هذا الملف في *خوادمه الخاصة على الإنترنت*، وليس في جهازكِ الشخصي. وبما أن الصورة موجودة في جهازكِ فقط، لا يتمكن المتصفح من العثور عليها.



**Phase 3: Styling Your Web Page**
**لمرحلة 3: تزيين وتنسيق صفحتكِ بالـ CSS**

To make our page look attractive, I added inline styling to the `<body>` and `<h1>` tags to apply background and text colors.


لتبدو الصفحة جذابة، اضفت تنسيقات داخلية (Inline CSS) لوسوم الـ `<body>` والـ `<h1>` لتغيير ألوان الخلفية والنصوص.

```html
<body style="background-color: Lavender;">
    <h1 style="background-color: MediumPurple;">Taleen sami alharbi</h1>
    ...
</body>

```

This gives the page a beautiful lavender background and highlights the header with a medium purple block.


يعطي هذا التعديل خلفية هادئة بلون الخزامى (Lavender) مع إبراز شريط العنوان بلون بنفسجي متوسط (MediumPurple).



**Phase 4: Publishing to a Live Host (InfinityFree)**
  **المرحلة 4: نشر الموقع على استضافة حية (InfinityFree)**

To share my page with the world, I deployed it to a real, free web hosting provider: **InfinityFree**.


لمشاركة صفحتي مع العالم، قمت برفعها على استضافة ويب حقيقية ومجانية وهي **InfinityFree**.

**Step 1: Accessing the File Manager**
 **الدخول إلى مدير الملفات**

 - Log into your InfinityFree hosting panel and open the **File Manager**.

- سجل الدخول إلى لوحة استضافة InfinityFree وافتح **File Manager**.

 - Double-click and enter the **`htdocs`** folder. (This is the public folder where all website files must live).

- اضغط مرتين للدخول إلى مجلد **`htdocs`** (هذا هو المجلد العام الذي يجب أن توضع فيه جميع ملفات موقعكِ ليراها الزوار).

 **Step 2: Renaming to `index.html`** 
 **إعادة تسمية الملف إلى `index.html`**

 Web servers always look for a file named `index.html` as the default homepage. I rename my `Taleen.html` file to **`index.html`** before uploading.


تبحث خوادم الويب دائماً عن ملف باسم `index.html` ليكون الصفحة الرئيسية للموقع بشكل تلقائي. لذا قمت بتعديل اسم ملفي من `Taleen.html` إلى **`index.html`**.

 **Step 3: Uploading the Files** 
 **رفع الملفات إلى الاستضافة**

- Upload the **`index.html`** file into the `htdocs` folder.

- ارفع ملف **`index.html`** داخل مجلد `htdocs`.

- Upload the **`silly-cat.png`** image file into the **same** `htdocs` folder.

- ارفع ملف الصورة **`silly-cat.png`** داخل **نفس المجلد** `htdocs` بجانب ملف الكود.

>  **Why? / لماذا؟**
> If you only upload the HTML code, the server won't have access to the physical picture file. Uploading both to the same root folder satisfies the relative link `src="silly-cat.png"`.


> إذا رفعتِ كود الـ HTML فقط، لن يجد الخادم ملف الصورة الفعلي لعرضه. رفع الملفين معاً في نفس المجلد يحقق شروط الرابط النسبي بنجاح.

---

**Phase 5: Success! Your Site is Live**
  **المرحلة 5: النجاح! موقعكِ الآن مباشر على الإنترنت**

 Open your web browser and navigate to your domain (e.g., `[https://taleen.free.je](https://taleen.free.je)`).


افتح متصفح الويب واكتبي رابط موقعكِ الخاص (مثال: `[https://taleen.free.je](https://taleen.free.je)`).

 **Result:** The live server successfully reads the code, fetches the styled header, reads `silly-cat.png` from the folder, and displays a fully functioning website on the internet!


يقرأ الخادم الحي الكود بنجاح، ويجلب الألوان والتنسيقات، ثم يسحب صورة القط اللطيف من نفس المجلد ليعرض موقعاً متكاملاً يعمل بكفاءة أمام زوار الشبكة العالمية!
