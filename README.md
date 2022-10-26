# Load Torch Saved Files Ignoring The Tensors

Reads from a file created by `torch.save` but ignores everything but the basic builtins.

This allows one to extract a lot of the info present in a `torch.save` without having to wait a long time for the file to load.

### Usage - Command line:

The following prints the output to the terminal using Python Rich:

```bash
python act.py path_to_save_file.pt
```


### Usage - From Python
```python
import act

config = act.from_path_or_bytesio("the_path_to_the_thing.pt")

print(config["epochs"])
```


