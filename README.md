# Book_for_read

    


# Important Books Repository

very important books
the feature's : 


### Get Book Information

```java
public BookInfo getBookInfo(String book) {
        ArrayList<Book> repository = this.github.getBooksForRead();
        for(int i = 0; i < repository.size(); i++) {
            Book currentBook = repository.get(i);
            if(currentBook.getName().equals(book)) {
                boolean isFinished = currentBook.isFinished();
                int currentPage = currentBook.getCurrentPage();
                return new BookInfo(isFinished, currentPage);
            }
        }
        
        return new BookInfo(false, -1);
    }
```

- getBookInfo(book)=>{true,123}
