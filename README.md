# LibraryProject

This is a Django starter project for the **Introduction to Django** lab.

## Steps Completed
- Installed Django
- Created project: LibraryProject
- Applied initial migrations
- Ran development server (http://127.0.0.1:8000)

from django.db import models

class Book(models.Model):
    title = models.CharField(max_length=200)
    author = models.CharField(max_length=100)
    published_date = models.DateField()
    isbn = models.CharField(max_length=13, unique=True)

    def __str__(self):
        return f"{self.title} by {self.author}"

