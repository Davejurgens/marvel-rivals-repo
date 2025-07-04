# Marvel Rivals Ranking Service API

![alt text](../media/Cover_5.png)

This is a mock API to simulate the REST interface of an imaginary service.

The Marvels Rivals Rankings API lets you search for a comic in the database. Use this API service to:
- Get a list of all superheroes or a specific superhero by character name from the database.
- Add a superhero character to the database.
- Update a supehero character in the database.
- Retrieve the following details for each superhero in the database:
    - `issueNumber`: The specific issue number of the book.
    - `publisher`: The company that published the book.
    - `date`: The publication date of the book.
    - `conditionGrade`: The grade indicating the condition of the book.
    - `status`: The status of the comic book (e.g., Restored).
    - `upcCode`: The unique product code for the comic book.
    - `tradePrice`: The trade price of the comic book.
    - `currency`: The currency of the trade price.

## Tutorials

First, do this tutorial to set up your development system for these tutorials. You only have to do this one time per development system.

* [Setting up your development system](https://github.com/KusumaKrish15/Comic-Database-Service/blob/main/docs/tutorials/dev-env.md)

After your system is ready, these tutorials show you how to perform common tasks.
- [Getting started with the Comic Database Service API](https://github.com/KusumaKrish15/Comic-Database-Service/blob/main/docs/tutorials/Getting_started.md)
- [Add a new comic to the database](https://github.com/KusumaKrish15/Comic-Database-Service/blob/main/docs/tutorials/Add_a_new_comic.md)
- [Update an existing comic in the database](https://github.com/KusumaKrish15/Comic-Database-Service/blob/main/docs/tutorials/Update_a_comic.md)

## API reference docs

The API References show detailed descriptions of the service's resources.

The API reference docs refer to a `{base_url}` when they
refer to the URL of a resource. The `{base_url}` value depends
on the installation of the service.

When run locally for testing, the `{base_url}` is
generally `http://localhost:3000`.

- [Get a list of comic books](https://github.com/KusumaKrish15/Comic-Database-Service/blob/main/docs/api/Get-comics.md)
- [Get a list of comic trade paperback books](https://github.com/KusumaKrish15/Comic-Database-Service/blob/main/docs/api/Get-comics-paperback.md)
- [Add a new comic book](https://github.com/KusumaKrish15/Comic-Database-Service/blob/main/docs/api/Post-comic.md)
- [Add a new comic trade paperback book](https://github.com/KusumaKrish15/Comic-Database-Service/blob/main/docs/api/Post-comic-paperback.md)

## API resources

These API resources and endpoints are available:
- [comicBook](https://github.com/KusumaKrish15/Comic-Database-Service/blob/main/docs/api/comicBook.md)
- [comicTradePaperBack](https://github.com/KusumaKrish15/Comic-Database-Service/blob/main/docs/api/comicTradePaperBack.md)
