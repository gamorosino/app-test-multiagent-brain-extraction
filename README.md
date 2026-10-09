# app-test-multiagent-brain-extraction

Skull-strip a T1w volume with FSL's bet

## Inputs

- `t1` (neuro/nifti)

## Outputs

- `out` (neuro/nifti) -- 

## Usage

Brainlife.io: run via `braise-app-run`/`braise-app-pipeline` (once registered
with `braise-app-create`), or the web UI.

Locally (outside brainlife): copy `config.json.example` to `config.json`,
fill in real file paths, then run `./main` from this directory. `main` pulls
its own container (`singularity exec docker://...`) -- no local install of
the underlying tool needed, only Singularity itself.

Entrypoint: `brain_extract.py`

## Authors

- Gabriele Amorosino <g.amorosino@gmail.com>

## License

MIT, see `LICENSE`.
