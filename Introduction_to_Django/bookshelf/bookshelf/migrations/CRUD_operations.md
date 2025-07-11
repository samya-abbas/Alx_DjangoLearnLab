```python
# Create a Book instance
from bookshelf.models import Book
book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)
book
# <Book: 1984 by George Orwell (1949)>

### 📄 `retrieve.md`
```python
# Retrieve and display all attributes of the book
from bookshelf.models import Book
book = Book.objects.get(title="1984")
book.title           # '1984'
book.author          # 'George Orwell'
book.publication_year  # 1949



### 📄 `update.md`
```python
# Update the title of the book and save
from bookshelf.models import Book
book = Book.objects.get(title="1984")
book.title = "Nineteen Eighty-Four"
book.save()
book.title  # 'Nineteen Eighty-Four'

```python
# Delete the book instance
from bookshelf.models import Book
book = Book.objects.get(title="Nineteen Eighty-Four")
book.delete()

# Confirm deletion
Book.objects.all()
# <QuerySet []>