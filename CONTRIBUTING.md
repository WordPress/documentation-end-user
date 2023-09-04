## Add another language

If you wish to translate WordPress documentation to langunage that doesn't exist in this repository, first you have to add the language to the repository. 

1. Fork the entire repository to your own account. 
2. Clone your repository to your local machine. 
    - `git clone git@github.com:<user>/documentation-end-user.git` 
3. Navigate to repository's folder 
    - `cd documentation-end-user`
4. Create a new branch 
    - `git chekout -b add/language-<language_name>`
5. Create a new forlder named by the new [language code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) 
    - `mkdir <language>`
6. Copy all files and folders from `en` folder to the new language folder 
    - `cp -r en/* <language>/`
7. Make a copy of English manifest file and rename it for the new language 
    - `cp manifest/documentation-manifest-en.json manifest/documentation-manifest-<language>.json`
8. Translate the following line to the new language and add it to [README.md](https://github.com/WordPress/documentation-end-user/blob/trunk/README.md#languages):
    - `[EN - English](en/): Check the documentation in English..` 
9. Add, commit and push changes to your GitHub repository 
    - `git add .`
    - `git commit -m "Add <language_name> language."`
    - `git push origin add/language-<language_name>`
10. Through GitHub create a pull request from your `add/language-<language_name>` branch to `trunk` branch in WordPress/documentation-end-user repo.
11. Wait for someone to review, approve and merge your request.
