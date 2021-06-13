# DJANGO PROJECT TEMPLATE

## Technologies
 - Python 3.9.5
 - Poetry 1.1.6
 - Django 3.2.4
 - DRF 3.12.4
 - gunicorn 20.1.0
 - Docker 20.10.7
 - Docker Compose 1.29.2
 - Postgres 13.3
 - NGINX 1.21.0
 
## QUICKSTART
 - install "Docker" and "Docker Compose"
 - create and fill dev.env or prod.env with .env.template 
 - docker-compose up -d --build
    - for dev version add "-f docker-compose.dev.yml" after "docker-compose"
    - go into backend container and run ./manage.py migrate

## TIPS
 - use /docker catalog for nginx, redis, and so on...


## GIT STYLE
### Branch sample:
 - **Schema**: type/subject
 - **Example**: feature/login_module

### Commit sample:
 - **Schema**:
   - Type(optional scope): subject
 - **Example**: 
   - Feat(parser): add the ability to parse arrays
   - fix(middleware): ensure Range headers adhere more closely to RFC 2616

## Types:
 - Feat - A new feature
 - Fix - A bug fix
 - Refactor - A code change that neither fixes a bug or adds a feature
 - Perf - A code change that improves performance
 - Revert - Reverting things
 - Style - Markup, white-space, formatting, missing semi-colons...
 - Test - Adding missing tests
 - Docs - Documentation only changes
 - CI - CI related changes
 - Chore - Build process or auxiliary tool changes

## Subject:
 - Use the imperative, present tense: "change" not "changed" nor "changes"
 - No dot (.) at the end.

## Scope:
 - A scope may be provided to a commit’s type, to provide additional contextual information
 - and is contained within parenthesis, e.g., feat(parser): add ability to parse arrays.

##The rules of a great commit message:
 - Separate subject from body with a blank line
 - Limit the subject line to 50 characters
 - Summary in present tense. Not capitalized
 - Do not end the subject line with a period
 - Use the imperative mood in the subject line
