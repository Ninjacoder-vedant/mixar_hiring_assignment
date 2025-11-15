## How to run the code?
To view the results correctly, make sure to run each cell in the notebook in sequence.

* **`main.ipynb`** contains the code for the first three tasks.
* **`bonus_task.ipynb`** contains the code for the bonus task.

### Folder structure

* **`8samples/`**: contains the original 8 given meshes.
* **`normalized/`**: contains all meshes in their normalized form for both methods: *min-max* and *unit-sphere*.
* **`quantized/`**: contains all meshes in their quantized form for both methods: *min-max* and *unit-sphere*.
* **`reconstructed/`**: contains the reconstructed mesh obtained from the quantized version of `branch.obj`
* **`report.pdf`**: Summarizes all the end-to-end results for each task

## What .obj file contains?
| Keyword | Meaning            | Example                     | Explanation                    |
| ------- | ------------------ | --------------------------- | ------------------------------ |
| `v`     | Vertex             | `v x y z`                   | 3D coordinates (geometry)      |
| `vn`    | Vertex normal      | `vn nx ny nz`               | Direction vector for lighting  |
| `vt`    | Texture coordinate | `vt u v`                    | Mapping to 2D texture (UV map) |
| `f`     | Face               | `f v/vt/vn v/vt/vn v/vt/vn` | Triangles built from indices   |

**Key Results:**
- Unit sphere normalization preserves shape
- Min-max normalization has lower recontruction error