# campi-flegrei.datasette.stefan-dev.de

[![Vercel](../../actions/workflows/vercel.yml/badge.svg)](../../actions/workflows/vercel.yml)

Datasette with volcanic activities of the [Phlegraean Fields](https://en.wikipedia.org/wiki/Phlegraean_Fields).

## ⚙️ Get Started

You'll need [Datasette](https://datasette.io/) and [Python](https://python.org) installed.

### Clone Repository

First of all, you need to clone the repository:

```bash
$ git clone https://github.com/bystefankuehnel/campi-flegrei.datasette.stefan-dev.de.git
$ cd campi-flegrei.datasette.stefan-dev.de
```

### Install PIP Dependencies

```bash
$ python -m pip install --upgrade pip
$ pip install -r requirements.txt
```

### Download SQLite Database

```bash
$ curl \
    --silent \
    --show-error \
    --location \
    --output events.db \
    https://campi-flegrei.datasette.stefan-dev.de/events.db
```

### Run Datasette

```bash
$ datasette events.db \
    --metadata metadata.json \
    --open
```

It will listen on [http://127.0.0.1:8001](http://127.0.0.1:8001) unless otherwise configured.

## 🔨 Technology

The following technologies, tools and platforms were used during development.

- **Code**: [Python](https://www.python.org)
- **Database**: [SQLite](https://sqlite.org)
- **Deployment**: [Vercel](https://vercel.com)

## 👷‍ Error Found?

Thank you for your message! Please fill out a [bug report](../../issues/new?assignees=&labels=&template=bug_report.md&title=).

## License

This project is licensed under the [European Union Public License 1.2](https://choosealicense.com/licenses/eupl-1.2/).
