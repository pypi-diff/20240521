# Comparing `tmp/alphafold3_pytorch-0.0.5.tar.gz` & `tmp/alphafold3_pytorch-0.0.6.tar.gz`

## Comparing `alphafold3_pytorch-0.0.5.tar` & `alphafold3_pytorch-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/.env.sample
--rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/alphafold3.png
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/contribute.sh
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/.github/workflows/test.yml
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/alphafold3_pytorch/__init__.py
--rw-r--r--   0        0        0    71221 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/alphafold3_pytorch/alphafold3.py
--rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/alphafold3_pytorch/attention.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/alphafold3_pytorch/typing.py
--rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/docs/alphafold3-supplementary.pdf
--rw-r--r--   0        0        0     9308 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/tests/test_af3.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/LICENSE
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/README.md
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     6435 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/.env.sample
+-rw-r--r--   0        0        0   248685 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/alphafold3.png
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/contribute.sh
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/alphafold3_pytorch/__init__.py
+-rw-r--r--   0        0        0    79473 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/alphafold3_pytorch/alphafold3.py
+-rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/alphafold3_pytorch/attention.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/alphafold3_pytorch/typing.py
+-rw-r--r--   0        0        0   584890 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/docs/alphafold3-supplementary.pdf
+-rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/tests/test_af3.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/README.md
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 alphafold3_pytorch-0.0.6/PKG-INFO
```

### Comparing `alphafold3_pytorch-0.0.5/alphafold3.png` & `alphafold3_pytorch-0.0.6/alphafold3.png`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.5/.github/workflows/publish.yml` & `alphafold3_pytorch-0.0.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.5/alphafold3_pytorch/alphafold3.py` & `alphafold3_pytorch-0.0.6/alphafold3_pytorch/alphafold3.py`

 * *Files 5% similar despite different names*

```diff
@@ -1746,14 +1746,245 @@
             loss = loss + smooth_lddt_loss
 
         if not return_denoised_pos:
             return loss
 
         return loss, denoised
 
+
+# modules todo
+
+class SmoothLDDTLoss(Module):
+    """ Algorithm 27 """
+
+    @typecheck
+    def __init__(self, nucleic_acid_cutoff: float = 30.0, other_cutoff: float = 15.0):
+        super().__init__()
+        self.nucleic_acid_cutoff = nucleic_acid_cutoff
+        self.other_cutoff = other_cutoff
+
+    @typecheck
+    def forward(
+        self,
+        pred_coords: Float['b n 3'],
+        true_coords: Float['b n 3'],
+        is_dna: Bool['b n'],
+        is_rna: Bool['b n']
+    ) -> Float['']:
+        """
+        pred_coords: predicted coordinates (b, n, 3)
+        true_coords: true coordinates (b, n, 3)
+        is_dna: boolean tensor indicating DNA atoms (b, n)
+        is_rna: boolean tensor indicating RNA atoms (b, n)
+        """
+        # Compute distances between all pairs of atoms
+        pred_dists = torch.cdist(pred_coords, pred_coords)
+        true_dists = torch.cdist(true_coords, true_coords)
+
+        # Compute distance difference for all pairs of atoms
+        dist_diff = torch.abs(true_dists - pred_dists)
+
+        # Compute epsilon values
+        eps = (
+            F.sigmoid(0.5 - dist_diff) +
+            F.sigmoid(1.0 - dist_diff) +
+            F.sigmoid(2.0 - dist_diff) +
+            F.sigmoid(4.0 - dist_diff)
+        ) / 4.0
+
+        # Restrict to bespoke inclusion radius
+        is_nucleotide = is_dna | is_rna
+        is_nucleotide_pair = is_nucleotide.unsqueeze(-1) & is_nucleotide.unsqueeze(-2)
+        inclusion_radius = torch.where(
+            is_nucleotide_pair,
+            true_dists < self.nucleic_acid_cutoff,
+            true_dists < self.other_cutoff
+        )
+
+        # Compute mean, avoiding self term
+        mask = torch.logical_and(inclusion_radius, torch.logical_not(torch.eye(pred_coords.shape[1], dtype=torch.bool, device=pred_coords.device)))
+        lddt_sum = (eps * mask).sum(dim=(-1, -2))
+        lddt_count = mask.sum(dim=(-1, -2))
+        lddt = lddt_sum / lddt_count.clamp(min=1)
+
+        return 1 - lddt.mean()
+
+class WeightedRigidAlign(Module):
+    """ Algorithm 28 """
+    def __init__(self):
+        super().__init__()
+
+    @typecheck
+    def forward(
+        self,
+        pred_coords: Float['b n 3'],
+        true_coords: Float['b n 3'],
+        weights: Float['b n']
+    ) -> Float['b n 3']:
+        """
+        pred_coords: predicted coordinates (b, n, 3)
+        true_coords: true coordinates (b, n, 3)
+        weights: weights for each atom (b, n)
+        """
+        # Compute weighted centroids
+        pred_centroid = (pred_coords * weights.unsqueeze(-1)).sum(dim=1) / weights.sum(dim=1, keepdim=True)
+        true_centroid = (true_coords * weights.unsqueeze(-1)).sum(dim=1) / weights.sum(dim=1, keepdim=True)
+
+        # Center the coordinates
+        pred_coords_centered = pred_coords - pred_centroid.unsqueeze(1)
+        true_coords_centered = true_coords - true_centroid.unsqueeze(1)
+
+        # Compute the weighted covariance matrix
+        cov_matrix = torch.einsum('bni,bnj->bij', true_coords_centered * weights.unsqueeze(-1), pred_coords_centered)
+
+        # Compute the SVD of the covariance matrix
+        U, _, V = torch.svd(cov_matrix)
+
+        # Compute the rotation matrix
+        rot_matrix = torch.einsum('bij,bjk->bik', U, V)
+
+        # Ensure proper rotation matrix with determinant 1
+        det = torch.det(rot_matrix)
+        det_mask = det < 0
+        V_fixed = V.clone()
+        V_fixed[det_mask, :, -1] *= -1
+        rot_matrix[det_mask] = torch.einsum('bij,bjk->bik', U[det_mask], V_fixed[det_mask])
+
+        # Apply the rotation and translation
+        aligned_coords = torch.einsum('bni,bij->bnj', pred_coords_centered, rot_matrix) + true_centroid.unsqueeze(1)
+
+        return aligned_coords.detach()
+
+class ExpressCoordinatesInFrame(Module):
+    """ Algorithm  29 """
+
+    def __init__(self, eps = 1e-8):
+        super().__init__()
+        self.eps = eps
+
+    @typecheck
+    def forward(
+        self,
+        coords: Float['b m 3'],
+        frame: Float['b m 3 3']
+    ) -> Float['b m 3']:
+        """
+        coords: coordinates to be expressed in the given frame (b, 3)
+        frame: frame defined by three points (b, 3, 3)
+        """
+
+        # Extract frame points
+        a, b, c = frame.unbind(dim = -1)
+
+        # Compute unit vectors of the frame
+        e1 = F.normalize(a - b, dim = -1, eps = self.eps)
+        e2 = F.normalize(c - b, dim = -1, eps = self.eps)
+        e3 = torch.cross(e1, e2, dim = -1)
+
+        # Express coordinates in the frame basis
+        v = coords - b
+
+        transformed_coords = torch.stack([
+            einsum(v, e1, '... i, ... i -> ...'),
+            einsum(v, e2, '... i, ... i -> ...'),
+            einsum(v, e3, '... i, ... i -> ...')
+        ], dim = -1)
+
+        return transformed_coords
+
+class ComputeAlignmentError(Module):
+    """ Algorithm 30 """
+    @typecheck
+    def __init__(self, eps: float = 1e-8):
+        super().__init__()
+        self.eps = eps
+        self.express_coordinates_in_frame = ExpressCoordinatesInFrame()
+
+    @typecheck
+    def forward(
+        self,
+        pred_coords: Float['b n 3'],
+        true_coords: Float['b n 3'],
+        pred_frames: Float['b n 3 3'],
+        true_frames: Float['b n 3 3']
+    ) -> Float['b n']:
+        """
+        pred_coords: predicted coordinates (b, n, 3)
+        true_coords: true coordinates (b, n, 3)
+        pred_frames: predicted frames (b, n, 3, 3)
+        true_frames: true frames (b, n, 3, 3)
+        """
+        # Express predicted coordinates in predicted frames
+        pred_coords_transformed = self.express_coordinates_in_frame(pred_coords, pred_frames)
+
+        # Express true coordinates in true frames
+        true_coords_transformed = self.express_coordinates_in_frame(true_coords, true_frames)
+
+        # Compute alignment errors
+        alignment_errors = torch.sqrt(
+            torch.sum((pred_coords_transformed - true_coords_transformed) ** 2, dim=-1) + self.eps
+        )
+
+        return alignment_errors
+
+class CentreRandomAugmentation(Module):
+    """ Algorithm 19 """
+    @typecheck
+    def __init__(self, trans_scale: float = 1.0):
+        super().__init__()
+        self.trans_scale = trans_scale
+
+    @typecheck
+    def forward(self, coords: Float['b n 3']) -> Float['b n 3']:
+        """
+        coords: coordinates to be augmented (b, n, 3)
+        """
+        # Center the coordinates
+        centered_coords = coords - coords.mean(dim=1, keepdim=True)
+
+        # Generate random rotation matrix
+        rotation_matrix = self._random_rotation_matrix(coords.device)
+
+        # Generate random translation vector
+        translation_vector = self._random_translation_vector(coords.device)
+
+        # Apply rotation and translation
+        augmented_coords = torch.einsum('bni,ij->bnj', centered_coords, rotation_matrix) + translation_vector
+
+        return augmented_coords
+
+    @typecheck
+    def _random_rotation_matrix(self, device: torch.device) -> Float['3 3']:
+        # Generate random rotation angles
+        angles = torch.rand(3, device=device) * 2 * torch.pi
+
+        # Compute sine and cosine of angles
+        sin_angles = torch.sin(angles)
+        cos_angles = torch.cos(angles)
+
+        # Construct rotation matrix
+        rotation_matrix = torch.eye(3, device=device)
+        rotation_matrix[0, 0] = cos_angles[0] * cos_angles[1]
+        rotation_matrix[0, 1] = cos_angles[0] * sin_angles[1] * sin_angles[2] - sin_angles[0] * cos_angles[2]
+        rotation_matrix[0, 2] = cos_angles[0] * sin_angles[1] * cos_angles[2] + sin_angles[0] * sin_angles[2]
+        rotation_matrix[1, 0] = sin_angles[0] * cos_angles[1]
+        rotation_matrix[1, 1] = sin_angles[0] * sin_angles[1] * sin_angles[2] + cos_angles[0] * cos_angles[2]
+        rotation_matrix[1, 2] = sin_angles[0] * sin_angles[1] * cos_angles[2] - cos_angles[0] * sin_angles[2]
+        rotation_matrix[2, 0] = -sin_angles[1]
+        rotation_matrix[2, 1] = cos_angles[1] * sin_angles[2]
+        rotation_matrix[2, 2] = cos_angles[1] * cos_angles[2]
+
+        return rotation_matrix
+
+    @typecheck
+    def _random_translation_vector(self, device: torch.device) -> Float['3']:
+        # Generate random translation vector
+        translation_vector = torch.randn(3, device=device) * self.trans_scale
+        return translation_vector
+
 # input embedder
 
 EmbeddedInputs = namedtuple('EmbeddedInputs', [
     'single_inputs',
     'single_init',
     'pairwise_init',
     'atom_feats',
```

### Comparing `alphafold3_pytorch-0.0.5/alphafold3_pytorch/attention.py` & `alphafold3_pytorch-0.0.6/alphafold3_pytorch/attention.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.5/alphafold3_pytorch/typing.py` & `alphafold3_pytorch-0.0.6/alphafold3_pytorch/typing.py`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.5/docs/alphafold3-supplementary.pdf` & `alphafold3_pytorch-0.0.6/docs/alphafold3-supplementary.pdf`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.5/tests/test_af3.py` & `alphafold3_pytorch-0.0.6/tests/test_af3.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import os
 os.environ['TYPECHECK'] = 'True'
 
 import torch
 import pytest
 
 from alphafold3_pytorch import (
+    SmoothLDDTLoss,
+    WeightedRigidAlign,
+    ExpressCoordinatesInFrame,
+    ComputeAlignmentError,
+    CentreRandomAugmentation,
     PairformerStack,
     MSAModule,
     DiffusionTransformer,
     DiffusionModule,
     ElucidatedAtomDiffusion,
     RelativePositionEncoding,
     TemplateEmbedder,
@@ -34,14 +39,68 @@
         ground_truth, 
         is_rna_per_atom, 
         is_dna_per_atom
     )
 
     assert torch.all(loss <= 1) and torch.all(loss >= 0)
 
+# ToDo tests
+
+def test_smooth_lddt_loss():
+    pred_coords = torch.randn(2, 100, 3)
+    true_coords = torch.randn(2, 100, 3)
+    is_dna = torch.randint(0, 2, (2, 100)).bool()
+    is_rna = torch.randint(0, 2, (2, 100)).bool()
+
+    loss_fn = SmoothLDDTLoss()
+    loss = loss_fn(pred_coords, true_coords, is_dna, is_rna)
+
+    assert loss.numel() == 1
+
+def test_weighted_rigid_align():
+    pred_coords = torch.randn(2, 100, 3)
+    true_coords = torch.randn(2, 100, 3)
+    weights = torch.rand(2, 100)
+
+    align_fn = WeightedRigidAlign()
+    aligned_coords = align_fn(pred_coords, true_coords, weights)
+
+    assert aligned_coords.shape == pred_coords.shape
+
+def test_express_coordinates_in_frame():
+    batch_size = 2
+    num_coords = 100
+    coords = torch.randn(batch_size, num_coords, 3)
+    frame = torch.randn(batch_size, num_coords, 3, 3)
+
+    express_fn = ExpressCoordinatesInFrame()
+    transformed_coords = express_fn(coords, frame)
+
+    assert transformed_coords.shape == (batch_size, num_coords, 3)
+
+def test_compute_alignment_error():
+    pred_coords = torch.randn(2, 100, 3)
+    true_coords = torch.randn(2, 100, 3)
+    pred_frames = torch.randn(2, 100, 3, 3)
+    true_frames = torch.randn(2, 100, 3, 3)
+
+    error_fn = ComputeAlignmentError()
+    alignment_errors = error_fn(pred_coords, true_coords, pred_frames, true_frames)
+
+    assert alignment_errors.shape == (2, 100)
+
+def test_centre_random_augmentation():
+    coords = torch.randn(2, 100, 3)
+
+    augmentation_fn = CentreRandomAugmentation()
+    augmented_coords = augmentation_fn(coords)
+
+    assert augmented_coords.shape == coords.shape
+
+
 def test_pairformer():
     single = torch.randn(2, 16, 384)
     pairwise = torch.randn(2, 16, 16, 128)
     mask = torch.randint(0, 2, (2, 16)).bool()
 
     pairformer = PairformerStack(
         depth = 4
```

### Comparing `alphafold3_pytorch-0.0.5/.gitignore` & `alphafold3_pytorch-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.5/LICENSE` & `alphafold3_pytorch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alphafold3_pytorch-0.0.5/README.md` & `alphafold3_pytorch-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 Getting a fair number of emails. You can chat with me about this work <a href="https://discord.gg/x6FuzQPQXY">here</a>
 
 ## Appreciation
 
 - <a href="https://github.com/joseph-c-kim">Joseph</a> for contributing the Relative Positional Encoding and the Smooth LDDT Loss!
 
+- <a href="https://github.com/engelberger">Felipe</a> for contributing Weighted Rigid Align, Express Coordinates In Frame, Compute Alignment Error, and Centre Random Augmentation modules!
+
 ## Install
 
 ```bash
 $ pip install alphafold3-pytorch
 ```
 
 ## Usage
```

#### html2text {}

```diff
@@ -1,31 +1,33 @@
 [./alphafold3.png]## Alphafold 3 - Pytorch (wip) Implementation of _A_l_p_h_a_f_o_l_d_ _3
 in Pytorch Getting a fair number of emails. You can chat with me about this
 work _h_e_r_e ## Appreciation - _J_o_s_e_p_h for contributing the Relative Positional
-Encoding and the Smooth LDDT Loss! ## Install ```bash $ pip install alphafold3-
-pytorch ``` ## Usage ```python import torch from alphafold3_pytorch import
-Alphafold3 alphafold3 = Alphafold3( dim_atom_inputs = 77,
-dim_additional_residue_feats = 33, dim_template_feats = 44 ) # mock inputs
-seq_len = 16 atom_seq_len = seq_len * 27 atom_inputs = torch.randn(2,
-atom_seq_len, 77) atom_mask = torch.ones((2, atom_seq_len)).bool()
-atompair_feats = torch.randn(2, atom_seq_len, atom_seq_len, 16)
-additional_residue_feats = torch.randn(2, seq_len, 33) template_feats =
-torch.randn(2, 2, seq_len, seq_len, 44) template_mask = torch.ones((2, 2)).bool
-() msa = torch.randn(2, 7, seq_len, 64) # required for training, but omitted on
-inference atom_pos = torch.randn(2, atom_seq_len, 3) residue_atom_indices =
-torch.randint(0, 27, (2, seq_len)) distance_labels = torch.randint(0, 37, (2,
-seq_len, seq_len)) pae_labels = torch.randint(0, 64, (2, seq_len, seq_len))
-pde_labels = torch.randint(0, 64, (2, seq_len, seq_len)) plddt_labels =
-torch.randint(0, 50, (2, seq_len)) resolved_labels = torch.randint(0, 2, (2,
-seq_len)) # train loss = alphafold3( num_recycling_steps = 2, atom_inputs =
-atom_inputs, atom_mask = atom_mask, atompair_feats = atompair_feats,
-additional_residue_feats = additional_residue_feats, msa = msa, templates =
-template_feats, template_mask = template_mask, atom_pos = atom_pos,
-residue_atom_indices = residue_atom_indices, distance_labels = distance_labels,
-pae_labels = pae_labels, pde_labels = pde_labels, plddt_labels = plddt_labels,
+Encoding and the Smooth LDDT Loss! - _F_e_l_i_p_e for contributing Weighted Rigid
+Align, Express Coordinates In Frame, Compute Alignment Error, and Centre Random
+Augmentation modules! ## Install ```bash $ pip install alphafold3-pytorch ```
+## Usage ```python import torch from alphafold3_pytorch import Alphafold3
+alphafold3 = Alphafold3( dim_atom_inputs = 77, dim_additional_residue_feats =
+33, dim_template_feats = 44 ) # mock inputs seq_len = 16 atom_seq_len = seq_len
+* 27 atom_inputs = torch.randn(2, atom_seq_len, 77) atom_mask = torch.ones((2,
+atom_seq_len)).bool() atompair_feats = torch.randn(2, atom_seq_len,
+atom_seq_len, 16) additional_residue_feats = torch.randn(2, seq_len, 33)
+template_feats = torch.randn(2, 2, seq_len, seq_len, 44) template_mask =
+torch.ones((2, 2)).bool() msa = torch.randn(2, 7, seq_len, 64) # required for
+training, but omitted on inference atom_pos = torch.randn(2, atom_seq_len, 3)
+residue_atom_indices = torch.randint(0, 27, (2, seq_len)) distance_labels =
+torch.randint(0, 37, (2, seq_len, seq_len)) pae_labels = torch.randint(0, 64,
+(2, seq_len, seq_len)) pde_labels = torch.randint(0, 64, (2, seq_len, seq_len))
+plddt_labels = torch.randint(0, 50, (2, seq_len)) resolved_labels =
+torch.randint(0, 2, (2, seq_len)) # train loss = alphafold3
+( num_recycling_steps = 2, atom_inputs = atom_inputs, atom_mask = atom_mask,
+atompair_feats = atompair_feats, additional_residue_feats =
+additional_residue_feats, msa = msa, templates = template_feats, template_mask
+= template_mask, atom_pos = atom_pos, residue_atom_indices =
+residue_atom_indices, distance_labels = distance_labels, pae_labels =
+pae_labels, pde_labels = pde_labels, plddt_labels = plddt_labels,
 resolved_labels = resolved_labels ) loss.backward() # after much training ...
 sampled_atom_pos = alphafold3( num_recycling_steps = 4, num_sample_steps = 16,
 atom_inputs = atom_inputs, atom_mask = atom_mask, atompair_feats =
 atompair_feats, additional_residue_feats = additional_residue_feats, msa = msa,
 templates = template_feats, template_mask = template_mask )
 sampled_atom_pos.shape # (2, 16 * 27, 3) ``` ## Contributing At the project
 root, run ```bash $ sh ./contribute.sh ``` Then, add your module to
```

### Comparing `alphafold3_pytorch-0.0.5/pyproject.toml` & `alphafold3_pytorch-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "alphafold3-pytorch"
-version = "0.0.5"
+version = "0.0.6"
 description = "Alphafold 3 - Pytorch"
 authors = [
     { name = "Phil Wang", email = "lucidrains@gmail.com" }
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
 license = { file = "LICENSE" }
```

### Comparing `alphafold3_pytorch-0.0.5/PKG-INFO` & `alphafold3_pytorch-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: alphafold3-pytorch
-Version: 0.0.5
+Version: 0.0.6
 Summary: Alphafold 3 - Pytorch
 Project-URL: Homepage, https://pypi.org/project/alphafold3-pytorch/
 Project-URL: Repository, https://github.com/lucidrains/alphafold3-pytorch
 Author-email: Phil Wang <lucidrains@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Phil Wang
@@ -54,14 +54,16 @@
 
 Getting a fair number of emails. You can chat with me about this work <a href="https://discord.gg/x6FuzQPQXY">here</a>
 
 ## Appreciation
 
 - <a href="https://github.com/joseph-c-kim">Joseph</a> for contributing the Relative Positional Encoding and the Smooth LDDT Loss!
 
+- <a href="https://github.com/engelberger">Felipe</a> for contributing Weighted Rigid Align, Express Coordinates In Frame, Compute Alignment Error, and Centre Random Augmentation modules!
+
 ## Install
 
 ```bash
 $ pip install alphafold3-pytorch
 ```
 
 ## Usage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.0.5 Summary:
+Metadata-Version: 2.3 Name: alphafold3-pytorch Version: 0.0.6 Summary:
 Alphafold 3 - Pytorch Project-URL: Homepage, https://pypi.org/project/
 alphafold3-pytorch/ Project-URL: Repository, https://github.com/lucidrains/
 alphafold3-pytorch Author-email: Phil Wang
 gmail.com> License: MIT License Copyright (c) 2024 Phil Wang Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -24,17 +24,19 @@
 Intelligence Requires-Python: >=3.8 Requires-Dist: beartype Requires-Dist:
 einops>=0.8.0 Requires-Dist: einx>=0.2.2 Requires-Dist: environs Requires-Dist:
 jaxtyping>=0.2.28 Requires-Dist: torch>=2.1 Requires-Dist: tqdm Provides-Extra:
 examples Provides-Extra: test Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown [./alphafold3.png]## Alphafold 3 -
 Pytorch (wip) Implementation of _A_l_p_h_a_f_o_l_d_ _3 in Pytorch Getting a fair number of
 emails. You can chat with me about this work _h_e_r_e ## Appreciation - _J_o_s_e_p_h for
-contributing the Relative Positional Encoding and the Smooth LDDT Loss! ##
-Install ```bash $ pip install alphafold3-pytorch ``` ## Usage ```python import
-torch from alphafold3_pytorch import Alphafold3 alphafold3 = Alphafold3
+contributing the Relative Positional Encoding and the Smooth LDDT Loss! -
+_F_e_l_i_p_e for contributing Weighted Rigid Align, Express Coordinates In Frame,
+Compute Alignment Error, and Centre Random Augmentation modules! ## Install
+```bash $ pip install alphafold3-pytorch ``` ## Usage ```python import torch
+from alphafold3_pytorch import Alphafold3 alphafold3 = Alphafold3
 ( dim_atom_inputs = 77, dim_additional_residue_feats = 33, dim_template_feats =
 44 ) # mock inputs seq_len = 16 atom_seq_len = seq_len * 27 atom_inputs =
 torch.randn(2, atom_seq_len, 77) atom_mask = torch.ones((2, atom_seq_len)).bool
 () atompair_feats = torch.randn(2, atom_seq_len, atom_seq_len, 16)
 additional_residue_feats = torch.randn(2, seq_len, 33) template_feats =
 torch.randn(2, 2, seq_len, seq_len, 44) template_mask = torch.ones((2, 2)).bool
 () msa = torch.randn(2, 7, seq_len, 64) # required for training, but omitted on
```

