# MLP Arcade

Six small browser games for teaching how a multilayer perceptron works, in teaching order:

1. **Be the Neuron** – compute a forward pass by hand (2 → 2 → 1, ReLU or sigmoid).
2. **Shape the Curve** – fit a target curve with three hidden neurons; see why linear activations can't bend.
3. **Blindfolded Hiker** – gradient descent on a hidden loss landscape; feel the learning rate.
4. **Blame Game** – backpropagation as credit assignment, in three levels (2, 4, then 6 weights).
5. **Separate the Dots** – decision boundaries on XOR, circles, moons and spirals; how many neurons are enough?
6. **Memorize vs Learn** – overfitting: train on 20 noisy points, then get scored on 40 you never saw.

Everything is a single file, `index.html`, with no build step and no dependencies beyond two Google Fonts (the page works without them). A tiny MLP trainer (Adam, full batch) lives inside the page.

## Run it

Open `index.html` in any modern browser, or host it with GitHub Pages:

1. Push this repository to GitHub.
2. Settings → Pages → Source: *Deploy from a branch* → branch `main`, folder `/ (root)`.
3. The site appears at `https://<your-user>.github.io/<repo-name>/`.

Each game has its own link, e.g. `…/#blame` or `…/#dots`, which is handy for putting one game on a slide.

## Classroom notes

- *Blindfolded Hiker*: gentle bowl with learning rate 1.8 / 2.0 / 2.1 shows a decaying zig-zag, a permanent bounce and divergence. Narrow canyon at 0.30 does the same on a steep valley.
- *Blame Game*: a perfect round unlocks the next level. The "Teacher" fold under the cheat sheet unlocks all levels at once for demos.
- *Memorize vs Learn*: the noise in the data has an error floor of about 0.045; three stars means the hidden-set error is close to it.

## License

MIT – see `LICENSE`.
