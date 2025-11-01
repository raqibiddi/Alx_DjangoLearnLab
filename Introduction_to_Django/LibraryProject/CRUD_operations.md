from bookshelf.models import Book
 
#For create operation

Python 3.13.7 (main, Aug 14 2025, 11:12:11) [Clang 17.0.0 (clang-1700.0.13.3)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
(InteractiveConsole)
>>> book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)
>>> book

# Output of above code

<Book: Book object (1)>

# For retrieve operation

>>> book = Book.objects.get(title="1984")

>>> book.title
>>> book.author
>>> book.publication_year

# Output of above code

'1984'
'George Orwell'
1949

# For update operation

>>> book.title = "Nineteen Eigthty-Four"
>>> book.save()
>>> book.title

# Output of above code

'Nineteen Eigthty-Four'

# For delete operation

>>> book.delete()
>>> Book.objects.all()

# Output of aboove code

(1, {'bookshelf.Book': 1})
<QuerySet []>
