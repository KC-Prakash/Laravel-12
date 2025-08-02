# Laravel 12

## 🔹 Laravel के हो?

Laravel एक PHP framework हो जसले web applications development लाई simplify र organize गर्छ। Taylor Otwell ले बनाएका हुन्, र यो framework ले clean code, scalability, र security लाई ध्यानमा राख्छ।  
Laravel एक open-source PHP framework हो जुन modern web applications बनाउन प्रयोग गरिन्छ। यो MVC (Model-View-Controller) architecture मा आधारित हुन्छ र web development लाई सजिलो, छरितो र organized बनाउँछ।

## ✅ Laravel का मुख्य विशेषताहरू (Key Features of Laravel):

### 1. 🔁 MVC Architecture Support
- Laravel ले Model-View-Controller (MVC) architecture प्रयोग गर्छ।
- यसले code लाई logically अलग गर्छ:
  - **Model** (डेटा)
  - **View** (UI)
  - **Controller** (logic)
- यसले application लाई maintainable र scalable बनाउँछ।

### 2. 📦 Eloquent ORM (Object Relational Mapper)
- Laravel को Eloquent ORM ले database को साथ interact गर्न modern र readable syntax दिन्छ।
- SQL लेख्न नपर्ने — model मार्फत डेटा fetch/insert/update गर्न सकिन्छ।
```php
// Example: सबै users ल्याउने
$users = User::all();
```

### 3. 🌐 Routing System
- Laravel ले clean र simple URL routing support गर्छ।
- Route ले URL लाई controller/function सँग जोड्छ।
```php
Route::get('/home', [HomeController::class, 'index']);
```

### 4. 🧠 Blade Templating Engine
- Blade एक powerful templating engine हो जसले PHP र HTML लाई मिलाएर dynamic views बनाउन मद्दत गर्छ।
```blade
<!-- resources/views/welcome.blade.php -->
<h1>Hello, {{ $name }}</h1>
```

### 5. 🔐 Security Features
- Laravel मा built-in security छ:
  - CSRF protection
  - XSS prevention
  - Password hashing (bcrypt, Argon2)
  - SQL injection prevention

### 6. ⚙️ Artisan Command Line Interface
- Artisan CLI ले command line बाट project create, migration, seeder, testing आदि सजिलै गर्न मिल्छ।
```bash
php artisan make:model Product -m
```

### 7. 🧪 Unit Testing Support
- Laravel ले PHPUnit integration संगै testing को राम्रो support दिन्छ।
- Application को logic verify गर्न automated test लेख्न मिल्छ।

### 8. 🗃️ Database Migration System
- Migration ले schema लाई version control गर्न मद्दत गर्छ।
- टिममा काम गर्दा database structure consistent राख्न helpful हुन्छ।

### 9. 📬 Email Integration
- Laravel ले विभिन्न drivers (SMTP, Mailgun, Postmark, etc.) प्रयोग गरेर email पठाउन सकिन्छ।

### 10. 🛠️ Queues and Background Jobs
- Heavy काम (email पठाउने, रिपोर्ट generate गर्ने, आदि) लाई queue मा राखेर background मा चलाउन सकिन्छ।

### 11. 📄 API Development
- Laravel RESTful API development को लागि धेरै उपयोगी छ।
- Resource controllers, API authentication (Passport, Sanctum) को support पनि छ।

### 12. 📂 File Storage System
- Laravel ले local, Amazon S3, Google Cloud Storage, आदि system हरूसँग file uploads र management support गर्छ।

### 13. 🌍 Localization (बहुभाषी Support)
- Multilingual apps बनाउन built-in localization feature प्रयोग गर्न सकिन्छ।

### 14. 🔄 Event Broadcasting & Real-Time Updates
- Laravel ले events र WebSockets को माध्यमबाट real-time features (जस्तै chat app, notifications) बनाउन support गर्छ।

## 🔹 किन Laravel प्रयोग गर्ने?
1. **MVC Architecture** – Code structured हुन्छ (Model, View, Controller अनुसार विभाजन हुन्छ)।
2. **Routing System** – User-friendly URL structure बनाउन सजिलो।
3. **Blade Templating Engine** – HTML मा PHP integrate गर्न सजिलो बनाउँछ।
4. **Eloquent ORM** – Database सँग interact गर्न modern र readable तरीका।
5. **Security Features** – CSRF, SQL injection prevention, hashing, etc.
6. **Authentication & Authorization** – Login, registration, roles, etc. छिटो बनाउन मिल्ने।
7. **Artisan CLI** – Command line बाट काम automate गर्न मिल्ने।
8. **Migration System** – Database schema version control।
9. **Testing Support** – PHPUnit आधारित testing system।

## 🔹 Laravel कुन कामका लागि उपयुक्त छ?
- eCommerce systems
- CMS (Content Management Systems)
- APIs/backend services
- SaaS products
- Blogs, portfolios, etc.

## ✅ Laravel Setup गर्न के-के चाहिन्छ?

Laravel चलाउनका लागि तपाईंलाई केही आवश्यक software/tools चाहिन्छ:

| **Tool** | **केको लागि?** |
|----------|-----------------|
| PHP (>= 8.1) | Laravel चलाउनको लागि |
| Composer | PHP dependencies manage गर्न |
| MySQL / MariaDB | Database को लागि |
| Node.js + NPM | CSS/JS compile गर्न (Vite प्रयोग गर्ने Laravel मा) |
| Code Editor (जस्तै VS Code) | कोड लेख्नको लागि |
| Web Server (Apache/Nginx) | Browser मा app देखाउन |
| Git (Optional) | Version control को लागि |

👉 तपाईंले XAMPP, Laragon, वा MAMP जस्ता tools ले यी सबै एकैपटक install गर्न सक्नुहुन्छ।

## ✅ XAMPP मा Laravel Setup कसरी गर्ने?

### 🔧 आवश्यक सामग्रीहरू:
1. ✅ XAMPP – Apache, PHP, MySQL install गर्नको लागि
2. ✅ Composer – Laravel download र manage गर्न
3. ✅ Laravel – Framework
4. ✅ Browser – App हेर्नको लागि
5. ✅ VS Code (optional, code लेख्न सजिलो)

### 🧱 Step-by-Step Process

#### 🔹 Step 1: XAMPP Download र Install गर्नुहोस्
👉 [XAMPP Website](https://www.apachefriends.org/) बाट डाउनलोड गरेर install गर्नुहोस्।
- Apache ✅
- MySQL ✅

**Apache Start गर्नु भन्दा पहिले:**
1. Apache -> Config -> PHP.ini मा Click गर्ने
2. NotePad मा Ctrl + F गरी Find Dialog Box Open गर्ने
3. निम्न extension मा लगाएको Comment हटाउने:
   - `extension=zip`
   - `extension=sodium`
   - `extension=intl`
   - `extension=gd`

**दुबै चालु गर्नुहोस्:**
- XAMPP Control Panel → Apache: Start
- MySQL: Start

#### 🔹 Step 2: Composer Install गर्नुहोस्
👉 [Composer Website](https://getcomposer.org/) बाट डाउनलोड गरेर install गर्नुहोस्।  
Install पछि `composer -V` चलाएर confirm गर्नुहोस्।

#### 🔹 Step 3: Laravel Project बनाउनुहोस्
अब Project बनाउने folder भित्र जानुहोस्:
1. Open VS Code
2. Terminal Open
3. Type: `composer global require laravel/installer`
4. Type: `laravel new ProjectName`
5. Project run हुन केही बिकल्प छान्नु वा उपयुक्त विकल्पमा Yes गर्दै जाने।
6. `cd ProjectName`
7. `composer run dev` वा `php artisan serve`
8. अब Browser मा जानुहोस्:
   - 👉 `http://127.0.0.1:8000` वा `http://localhost:8000`
   - Laravel को Welcome page देखिन्छ 🎉

#### 🔹 Step 5: Database Connection (MySQL)
1. Browser मा खोल्नुहोस् 👉 `http://localhost/phpmyadmin`
2. नयाँ Database बनाउनुहोस् नाम दिउँ `ProjectName_db`
3. `.env` फाइल खोल्नुहोस् र DB info राख्नुहोस्:
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=ProjectName_db
DB_USERNAME=root
DB_PASSWORD=
```
4. अब migration चलाउनुहोस्:
```bash
php artisan migrate
```

## Laravel 12 मा पूर्ण CRUD प्रणाली निर्माण गर्नुहोस्

### 🎯 CRUD को अर्थ:
- **C** – Create (डाटा थप्ने)
- **R** – Read (डाटा पढ्ने/हेर्ने)
- **U** – Update (डाटा सम्पादन गर्ने)
- **D** – Delete (डाटा हटाउने)

### 1. Model बनाउनुहोस्: ModelName
```bash
php artisan make:model ModelName
```
यो कमाण्डले `app/Models/ModelName.php` Model फाईल बनाउँछ।

```bash
php artisan make:model ModelName -m
```
यो कमाण्डले `app/Models/ModelName.php` Model र migration फाईल बनाउँछ।

#### Laravel मा Model बनाउने तरिकाहरू:
**1. Artisan Command को माध्यमबाट (सबैभन्दा सामान्य तरिका)**
```bash
php artisan make:model Product
```
यो कमाण्डले `app/Models/Product.php` फाइल बनाउँछ।  
👉 यदि साथमा migration, factory, seeder पनि बनाउन चाहनुहुन्छ भने:
```bash
php artisan make:model Product -mfsc
```
**Explanation:**
- `-m` = migration
- `-f` = factory
- `-s` = seeder
- `-c` = controller

**2. Manually फाइल बनाएर**
```php
<?php

namespace App\Models;

use Illuminate\Database\Eloquent\Model;

class Product extends Model
{
    // model को logic यहाँ लेख्न सकिन्छ
}
```
तर यो तरिका कम प्रयोग हुन्छ किनकि Artisan ले धेरै सजिलो बनाइदिन्छ।

**3. Using Stub Customization (Advanced customization)**
```bash
php artisan stub:publish
```
यसले `stubs/model.stub` फाइल बनाउँछ जसलाई edit गरेर भविष्यका सबै model हरू customized बनाइन्छ।

**Bonus: Model को Naming Conventions**
- Model सधैं **Singular** हुन्छ जस्तै: `Product`
- Table सधैं **Plural** हुन्छ जस्तै: `products`

### 📦 2. Migration लेख्नुहोस् र चलाउनुहोस्
`database/migrations/xxxx_create_model_names_table.php` खोल्नुहोस्:

#### Migration चलाउनुहोस्:
```bash
php artisan migrate
```

#### Laravel मा Migration बनाउने तरिकाहरू:
**1. Artisan Command को माध्यमबाट (सबैभन्दा सामान्य तरिका)**
```bash
php artisan make:migration create_products_table
```
यदि model सँगै बनाउने हो भने:
```bash
php artisan make:model Product -m
```
यसले `products` टेबलको migration file `database/migrations` भित्र बनाउँछ।

**2. Custom Table Name र Column Structure सहित**
```bash
php artisan make:migration create_orders_table --create=orders
```
Update table को लागि:
```bash
php artisan make:migration add_status_to_orders_table --table=orders
```
`--table=orders` भन्ने मतलब यो existing table को लागि हो।

**3. Manually Migration फाइल बनाउने**
```php
<?php

use Illuminate\Database\Migrations\Migration;
use Illuminate\Database\Schema\Blueprint;
use Illuminate\Support\Facades\Schema;

return new class extends Migration {
    public function up(): void
    {
        Schema::create('products', function (Blueprint $table) {
            $table->id();
            $table->string('name');
            $table->text('description')->nullable();
            $table->decimal('price', 8, 2);
            $table->timestamps();
        });
    }

    public function down(): void
    {
        Schema::dropIfExists('products');
    }
};
```

#### 🚀 Migration Run गर्ने
```bash
php artisan migrate
```
#### ❌ Migration Rollback गर्ने
```bash
php artisan migrate:rollback
```
#### 🔁 Reset सबै Migration
```bash
php artisan migrate:reset
```
#### 🔄 Refresh (Rollback + Re-run)
```bash
php artisan migrate:refresh
```
#### 📦 Fresh (Drop all tables and migrate again)
```bash
php artisan migrate:fresh
```

### 🧠 3. Model Configuration (fillable)
`app/Models/ModelName.php` मा:

#### ✅ 1. $fillable in Model
`$fillable` भन्नाले कुन fields mass assignment (form बाट एकैचोटि डाटा save गर्ने) गर्न मिल्छ भनेर Laravel लाई बताउँछ।
```php
namespace App\Models;

use Illuminate\Database\Eloquent\Model;

class Book extends Model
{
    protected $fillable = [
        'title',
        'author',
        'description',
        'price',
    ];
}
```
👉 यदि `$fillable` define नगरेको खण्डमा Laravel ले `MassAssignmentException` फाल्न सक्छ।

#### ✅ 2. Validation in Controller
Validation को काम user बाट आएको डाटा check गर्नु हो — input गलत भए error देखाउने।  
**📄 BookController.php**  
🔹 **store() method** (create गर्दा):
```php
public function store(Request $request)
{
    $validatedData = $request->validate([
        'title' => 'required|string|max:255',
        'author' => 'required|string|max:255',
        'description' => 'nullable|string',
        'price' => 'required|numeric|min:0',
    ]);

    Book::create($validatedData);

    return redirect()->route('books.index')->with('success', 'Book added successfully.');
}
```

🔹 **update() method** (edit गर्दा):
```php
public function update(Request $request, Book $book)
{
    $validatedData = $request->validate([
        'title' => 'required|string|max:255',
        'author' => 'required|string|max:255',
        'description' => 'nullable|string',
        'price' => 'required|numeric|min:0',
    ]);

    $book->update($validatedData);

    return redirect()->route('books.index')->with('success', 'Book updated successfully.');
}
```

#### 🔁 Summary Table
| **स्थान** | **के गरिन्छ** | **उद्देश्य** |
|------------|----------------|--------------|
| Model | `$fillable` array | कुन fields mass assign गर्न मिल्छ |
| Controller | `$request->validate([...])` | Form validation logic |

#### 🧪 Bonus Tip: Custom Validation Message
```php
$request->validate([
    'title' => 'required',
    'price' => 'required|numeric|min:0',
], [
    'title.required' => 'Please enter the book title.',
    'price.min' => 'Price must be at least 0.',
]);
```

**🤖 Laravel automatically handles:**
- Validation errors with `@error()` in Blade
- Old input values with `old('field_name')`

### 🎮 4. Controller बनाउनुहोस्
```bash
php artisan make:controller ModelNameController --resource
```
यसले `index`, `create`, `store`, `show`, `edit`, `update`, `destroy` method भएको controller बनाउँछ।  
`app/Http/Controllers/ModelNameController.php`:

#### Laravel मा Controller बनाउने तरिकाहरू:
**🟦 1. सामान्य Controller**
```bash
php artisan make:controller BookController
```
```php
class BookController extends Controller
{
    public function index() {
        // List books
    }

    public function customMethod() {
        // Custom logic
    }
}
```

**🟦 2. Resource Controller (Full CRUD Controller)**
```bash
php artisan make:controller BookController --resource
```
**Example Methods:**
```php
public function index() {}          // GET /books
public function create() {}         // GET /books/create
public function store(Request $r) {} // POST /books
public function show($id) {}        // GET /books/{id}
public function edit($id) {}        // GET /books/{id}/edit
public function update(Request $r, $id) {} // PUT/PATCH /books/{id}
public function destroy($id) {}     // DELETE /books/{id}
```

**🟦 3. API Resource Controller**
```bash
php artisan make:controller BookController --api
```
**Methods:** `index`, `store`, `show`, `update`, `destroy`

**🟦 4. Invokable Controller (Single Action)**
```bash
php artisan make:controller BookController --invokable
```
```php
class BookController extends Controller
{
    public function __invoke()
    {
        return 'This is a single action controller';
    }
}
```
**Route:**
```php
Route::get('/books', BookController::class);
```

**🟦 5. Controller in Subfolder / Namespace**
```bash
php artisan make:controller Admin/BookController --resource
```
**File Location:** `app/Http/Controllers/Admin/BookController.php`  
**Route Example:**
```php
use App\Http\Controllers\Admin\BookController;
Route::resource('admin/books', BookController::class);
```

#### 🔁 सारांश Table
| **प्रकार** | **Command** | **विशेषता** |
|-------------|-------------|--------------|
| सामान्य | `make:controller BookController` | मनपर्ने methods राख्न सकिने |
| Resource | `--resource` | Full CRUD methods |
| API Resource | `--api` | CRUD (form views बिना) |
| Invokable | `--invokable` | एक मात्र action (like `__invoke`) |
| Subfolder | `Admin/BookController` | Controller लाई organized राख्ने |

### 🌐 5. Routes define गर्नुहोस्
`routes/web.php` मा:

#### 📁 Route File: routes/web.php
यो फाइलमा हामी सबै Web-based Route हरु define गर्छौं।

#### 🔹 Laravel Routes Define गर्ने तरिका
**1. Basic Route (Single Action)**
```php
use App\Http\Controllers\BookController;

Route::get('/books', [BookController::class, 'index']);
Route::post('/books', [BookController::class, 'store']);
Route::get('/books/create', [BookController::class, 'create']);
Route::get('/books/{id}', [BookController::class, 'show']);
Route::get('/books/{id}/edit', [BookController::class, 'edit']);
Route::put('/books/{id}', [BookController::class, 'update']);
Route::delete('/books/{id}', [BookController::class, 'destroy']);
```

**2. Resource Route (Full CRUD Controller को लागि)**
```php
use App\Http\Controllers\BookController;

Route::resource('books', BookController::class);
```
यो एक लाइनले सबै CRUD routes create गर्छ।  
**Equivalent to:**
- GET `/books` → `index`
- GET `/books/create` → `create`
- POST `/books` → `store`
- GET `/books/{book}` → `show`
- GET `/books/{book}/edit` → `edit`
- PUT/PATCH `/books/{book}` → `update`
- DELETE `/books/{book}` → `destroy`

**3. API Resource Route**
```php
use App\Http\Controllers\Api\BookController;

Route::apiResource('books', BookController::class);
```
केवल API का लागि हो। `create` र `edit` method हटाइन्छ।

**4. Route Group with Prefix or Namespace**
```php
use App\Http\Controllers\Admin\BookController;

Route::prefix('admin')->name('admin.')->group(function () {
    Route::resource('books', BookController::class);
});
```
- **Route URL:** `/admin/books`
- **Route Name:** `admin.books.index`, `admin.books.store`, etc.

#### 🔁 Route Names Summary
| **Method** | **URI** | **Controller Method** | **Route Name** |
|------------|---------|-----------------------|----------------|
| GET | `/books` | `index()` | `books.index` |
| GET | `/books/create` | `create()` | `books.create` |
| POST | `/books` | `store()` | `books.store` |
| GET | `/books/{id}` | `show()` | `books.show` |
| GET | `/books/{id}/edit` | `edit()` | `books.edit` |
| PUT/PATCH | `/books/{id}` | `update()` | `books.update` |
| DELETE | `/books/{id}` | `destroy()` | `books.destroy` |

#### 🧪 Route Test गर्न
Browser वा Postman प्रयोग गर्न सक्नुहुन्छ:

| **Path** | **Method** | **Description** |
|----------|------------|-----------------|
| `/books` | GET | सबै पुस्तक देखाउने |
| `/books/create` | GET | नयाँ पुस्तकको फारम देखाउने |
| `/books` | POST | नयाँ पुस्तक स्टोर गर्ने |
| `/books/1` | GET | ID 1 भएको पुस्तक देखाउने |
| `/books/1/edit` | GET | ID 1 को पुस्तक सम्पादन फारम |
| `/books/1` | PUT/PATCH | ID 1 को पुस्तक अपडेट गर्ने |
| `/books/1` | DELETE | ID 1 को पुस्तक मेटाउने |

#### ✅ Route List हेर्न Command:
```bash
php artisan route:list
```

### 🎨 6. Views बनाउनुहोस्
**Folder structure:** `resources/views/modelname/`

#### **index.blade.php**
```blade
<h2>All ModelNames</h2>
<a href="{{ route('modelnames.create') }}">Create New</a>

@if(session('success'))
    <p>{{ session('success') }}</p>
@endif

<ul>
@foreach($modelnames as $model)
    <li>
        {{ $model->name }} |
        <a href="{{ route('modelnames.edit', $model->id) }}">Edit</a>
        <form action="{{ route('modelnames.destroy', $model->id) }}" method="POST" style="display:inline">
            @csrf
            @method('DELETE')
            <button type="submit">Delete</button>
        </form>
    </li>
@endforeach
</ul>
```

#### **create.blade.php**
```blade
<h2>Create ModelName</h2>
<form action="{{ route('modelnames.store') }}" method="POST">
    @csrf
    <input type="text" name="name" placeholder="Name" required>
    <textarea name="description" placeholder="Description"></textarea>
    <button type="submit">Create</button>
</form>
```

#### **edit.blade.php**
```blade
<h2>Edit ModelName</h2>
<form action="{{ route('modelnames.update', $modelname->id) }}" method="POST">
    @csrf
    @method('PUT')
    <input type="text" name="name" value="{{ $modelname->name }}" required>
    <textarea name="description">{{ $modelname->description }}</textarea>
    <button type="submit">Update</button>
</form>
```

### ✅ Summary:
| **Step** | **Description** |
|----------|-----------------|
| 1 | Model र Migration create |
| 2 | DB schema define र migrate |
| 3 | Controller CRUD method बनाउने |
| 4 | Route `resource()` द्वारा define |
| 5 | Blade views (index, create, edit) बनाउने |
| 6 | Validation र `$fillable` प्रयोग गर्ने |
