<h1 align="center">🧠 NeuralMind</h1>

<p align="center">
  Pixel-art creatures whose brains are real spiking neural networks.<br>
  They forage, fight, share, signal and evolve, and you can watch every neuron.
</p>

<p align="center">
  <a href="https://sitta07.github.io/NeuralMind/"><b>▶ Try it in your browser</b></a> ·
  <a href="#quickstart"><b>Quickstart</b></a> ·
  <a href="docs/GUIDE.md"><b>Guide</b></a> ·
  <a href="docs/research/FINDINGS.md"><b>Findings</b></a>
</p>

<p align="center">
  <img src="docs/media/evolution_world.gif" width="440" alt="An evolving population of spiking-neural agents">
  &nbsp;
  <img src="docs/media/brain_scanner.gif" width="300" alt="One agent's spiking network choosing its action, live">
</p>

## Quickstart

**No install:** open https://sitta07.github.io/NeuralMind/

**Run it locally** (Python 3.12+, no GPU, no API key):

```bash
git clone https://github.com/sitta07/NeuralMind.git && cd NeuralMind
pip install -r requirements-neuralmind.txt -r requirements-server.txt -r requirements-research.txt
python -m neuralmind.server     # open http://127.0.0.1:8000
```

Press **Play**, then click any creature to see its brain.

## Use it for

- **Watching brains:** the Playground at `/`
- **Research:** pre-registered studies in `studies/*.json`, results at `/lab` ([how to add one](docs/ADDING_A_STUDY.md))
- **RL:** a PettingZoo `ParallelEnv`:

```python
from neuralmind.envs import parallel_env
env = parallel_env(n_rl=4, n_snn=4, config={"social": True})
```

This is a computational model, not a real brain and not a conscious system ([evidence](docs/research/SCIENTIFIC_EVIDENCE.md)).

## Licence

[MIT](LICENSE). Pixel art: [Tiny Town](https://kenney.nl/assets/tiny-town) and [Tiny Dungeon](https://kenney.nl/assets/tiny-dungeon) by [Kenney](https://kenney.nl) (CC0). Details are in [`THIRD_PARTY_NOTICES.md`](THIRD_PARTY_NOTICES.md). To cite this work, use [`CITATION.cff`](CITATION.cff).
