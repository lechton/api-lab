## Open venv

`workon vintel`

## Check installations of venv

Once you've activated your virtual environment with `workon vintel`, you have a few options:

**The main command** is `pip list` — this shows every package installed in that virtual environment, along with its version number. So you run `pip list` and you get a neat table: package name on the left, version on the right.

**For more detail**, you can run `pip freeze` — this gives you the same information but formatted as a requirements file (each line reads like `fastapi==0.115.0`). This format is specifically designed so you could pipe it into a file with `pip freeze > requirements.txt` and later recreate the exact same environment elsewhere.

**To check a specific package**, say you want to know if FastAPI is installed, you run `pip show fastapi`. This gives you the version, summary, author, location on disk, and crucially — its dependencies (what other packages it requires) and what packages depend on *it*.

So in short: `pip list` for a quick overview, `pip freeze` for the exportable format, and `pip show <package_name>` to inspect one specific package.

## Install basic packages for FastAPI + Supabase project

`pip install fastapi uvicorn supabase python-dotenv`