from bookshelf.models import Book
 
#For create operation

Python 3.13.7 (main, Aug 14 2025, 11:12:11) [Clang 17.0.0 (clang-1700.0.13.3)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
(InteractiveConsole)
>>> book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)
>>> book

# Output of above code

<Book: Book object (1)>
