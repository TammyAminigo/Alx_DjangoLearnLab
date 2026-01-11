from bookshelf.models import Book
t = Book.objects.get(title="1984")
# Expected Output: <Book: 1984 by George Orwell>
