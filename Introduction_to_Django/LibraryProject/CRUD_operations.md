# CRUD Operations

## Create
```python
book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)
# Expected Output: <Book: 1984 by George Orwell>
```

## Retrieve
```python
t = Book.objects.get(title="1984")
# Expected Output: <Book: 1984 by George Orwell>
```

## Update
```python
book = Book.objects.get(title="1984")
book.title = "Nineteen Eighty-Four"
book.save()
# Expected Output: Nineteen Eighty-Four
```

## Delete
```python
book = Book.objects.get(title="Nineteen Eighty-Four")
book.delete()
# Expected Output: (1, {'bookshelf.Book': 1})
```
