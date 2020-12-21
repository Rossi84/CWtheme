# ConciliaWeb docs theme

This is the official theme for any piece of documentation of ConciliaWeb.

## How to use Sphinx CW theme on your documentation

* Add the following line to your documentation `requirements.txt` file:

    ```
    $ pip install git+https://github.com/Rossi84/CWtheme.git
    ```

* In your `conf.py` file, you'll need to specify the theme as follows:

    ```
    # Add this line at the top of the file within the "import" section
    import cw_theme

    # Add the Sphinx extension 'cw_theme' in the extensions list
    extensions = [
      ...,
      'cw_theme'
    ]

    # Edit these lines
    html_theme = "cw_theme"
    html_theme_path = [cw_theme.get_html_theme_path()]
    ```