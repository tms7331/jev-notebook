# Jev examples

This project is a hands-on introduction to TypeSafe AI's Jev decision model. The [notebook](jev_models.ipynb) explains its typed questions and probabilistic answers, makes a complete first API call, and walks through three useful workflows and three poor fits. The examples use Jev 1.13 through OpenRouter.

## Run the notebook

You'll need [uv](https://docs.astral.sh/uv/) and an OpenRouter API key with access to `typesafe/jev-1.13`.

1. From the repository root, install the Python environment:

   ```sh
   uv sync
   ```

2. Create a `.env` file in the repository root containing your key:

   ```text
   OPENROUTER_KEY=your_openrouter_key
   ```

   `.env` is ignored by Git. You can also set `OPENROUTER_KEY` in your shell instead.

3. Open `jev_models.ipynb` in VS Code or Jupyter and select the project's `.venv` Python kernel. If you need a Jupyter server, start one with:

   ```sh
   uv run --with jupyterlab jupyter lab jev_models.ipynb
   ```

4. Run the cells from top to bottom. Each example sends a live, billable request; the first prints the full request and response with the API key redacted.

For a single API call outside the notebook, run `uv run hello_jev.py`.
