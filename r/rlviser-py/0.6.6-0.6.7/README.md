# Comparing `tmp/rlviser_py-0.6.6.tar.gz` & `tmp/rlviser_py-0.6.7.tar.gz`

## Comparing `rlviser_py-0.6.6.tar` & `rlviser_py-0.6.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 rlviser_py-0.6.6/Cargo.toml
--rw-r--r--   0     1001      127     1070 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/LICENSE
--rw-r--r--   0     1001      127     1557 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/README.md
--rw-r--r--   0     1001      127     2873 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/gym_renderer.py
--rw-r--r--   0     1001      127     2547 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/pygymtest.py
--rw-r--r--   0     1001      127     2291 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/rlviser_py.pyi
--rw-r--r--   0     1001      127    18135 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/src/bytes.rs
--rw-r--r--   0     1001      127     5195 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/src/lib.rs
--rw-r--r--   0     1001      127     5462 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/src/socket.rs
--rw-r--r--   0     1001      127     8092 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/Cargo.lock
--rw-r--r--   0     1001      127      387 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 rlviser_py-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 rlviser_py-0.6.7/Cargo.toml
+-rw-r--r--   0     1001      127     1070 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/LICENSE
+-rw-r--r--   0     1001      127     1557 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/README.md
+-rw-r--r--   0     1001      127     2907 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/gym_renderer.py
+-rw-r--r--   0     1001      127     2547 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/pygymtest.py
+-rw-r--r--   0     1001      127     2291 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/rlviser_py.pyi
+-rw-r--r--   0     1001      127    18232 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/src/bytes.rs
+-rw-r--r--   0     1001      127     5195 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/src/lib.rs
+-rw-r--r--   0     1001      127     5462 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/src/socket.rs
+-rw-r--r--   0     1001      127     8092 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/Cargo.lock
+-rw-r--r--   0     1001      127      387 2024-05-17 07:09:37.000000 rlviser_py-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 rlviser_py-0.6.7/PKG-INFO
```

### Comparing `rlviser_py-0.6.6/Cargo.toml` & `rlviser_py-0.6.7/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rlviser-py"
-version = "0.6.6"
+version = "0.6.7"
 edition = "2021"
 description = "Python implementation that manages a UDP connection to RLViser"
 license = "MIT"
 repository = "https://github.com/VirxEC/rlviser-py"
 readme = "README.md"
 keywords = ["rlviser", "rocket-league", "udp", "python", "rlbot"]
 exclude = [".github", "pytest.py", "rustfmt.toml", ".gitignore"]
```

### Comparing `rlviser_py-0.6.6/LICENSE` & `rlviser_py-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.6/README.md` & `rlviser_py-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.6/gym_renderer.py` & `rlviser_py-0.6.7/gym_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         car_state.vel = rsim.Vec(*car.physics.linear_velocity)
         car_state.ang_vel = rsim.Vec(*car.physics.angular_velocity)
         car_state.rot_mat = rsim.RotMat(*car.physics.rotation_mtx.transpose().flatten())
 
         car_state.demo_respawn_timer = car.demo_respawn_timer
         car_state.is_on_ground = car.on_ground
         car_state.supersonic_time = car.supersonic_time
+        # print(car.boost_amount)
         car_state.boost = car.boost_amount * 100
         car_state.time_spent_boosting = car.boost_active_time
         car_state.handbrake_val = car.handbrake
 
         car_state.has_jumped = car.has_jumped
         car_state.last_controls.jump = car.is_holding_jump
         car_state.is_jumping = car.is_jumping
```

### Comparing `rlviser_py-0.6.6/pygymtest.py` & `rlviser_py-0.6.7/pygymtest.py`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.6/rlviser_py.pyi` & `rlviser_py-0.6.7/rlviser_py.pyi`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.6/src/bytes.rs` & `rlviser_py-0.6.7/src/bytes.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use pyo3::FromPyObject;
 
 #[repr(u8)]
 #[derive(Clone, Copy, Debug, Default)]
 pub enum GameMode {
     Soccar,
     Hoops,
-    Heatseeker,
+    HeatSeeker,
     Snowday,
     #[default]
     TheVoid,
 }
 
 #[derive(Clone, Copy, Debug, Default, FromPyObject)]
 pub struct Vec3 {
@@ -199,14 +199,15 @@
     pub has_double_jumped: bool,
     pub has_flipped: bool,
     pub flip_rel_torque: Vec3,
     pub jump_time: f32,
     pub flip_time: f32,
     pub is_flipping: bool,
     pub is_jumping: bool,
+    pub air_time: f32,
     pub air_time_since_jump: f32,
     pub boost: f32,
     pub time_spent_boosting: f32,
     pub is_supersonic: bool,
     pub supersonic_time: f32,
     pub handbrake_val: f32,
     pub is_auto_flipping: bool,
@@ -270,15 +271,14 @@
     pub tick_count: u64,
     pub tick_rate: f32,
     pub game_mode: GameMode,
     pub ball: BallState,
     pub pads: Vec<BoostPad>,
     pub cars: Vec<CarInfo>,
 }
-
 pub trait FromBytes {
     fn from_bytes(bytes: &[u8]) -> Self;
 }
 
 pub trait FromBytesExact: FromBytes {
     const NUM_BYTES: usize;
 }
@@ -290,14 +290,15 @@
 
 impl<'a> ByteReader<'a> {
     #[inline]
     pub const fn new(bytes: &'a [u8]) -> Self {
         Self { idx: 0, bytes }
     }
 
+    #[track_caller]
     pub fn read<I: FromBytesExact>(&mut self) -> I {
         let item = I::from_bytes(&self.bytes[self.idx..self.idx + I::NUM_BYTES]);
         self.idx += I::NUM_BYTES;
         item
     }
 
     #[inline]
@@ -419,15 +420,15 @@
 
 impl FromBytes for GameMode {
     #[inline]
     fn from_bytes(bytes: &[u8]) -> Self {
         match bytes[0] {
             0 => Self::Soccar,
             1 => Self::Hoops,
-            2 => Self::Heatseeker,
+            2 => Self::HeatSeeker,
             3 => Self::Snowday,
             4 => Self::TheVoid,
             _ => unreachable!(),
         }
     }
 }
 
@@ -457,15 +458,15 @@
 
         impl FromBytesExact for $t {
             const NUM_BYTES: usize = $n;
         }
     };
 }
 
-trait ToBytesExact<const N: usize>: FromBytesExact {
+pub trait ToBytesExact<const N: usize>: FromBytesExact {
     fn to_bytes(&self) -> [u8; N];
 }
 
 struct ByteWriter<const N: usize> {
     idx: usize,
     bytes: [u8; N],
 }
@@ -614,14 +615,15 @@
     has_double_jumped,
     has_flipped,
     flip_rel_torque,
     jump_time,
     flip_time,
     is_flipping,
     is_jumping,
+    air_time,
     air_time_since_jump,
     boost,
     time_spent_boosting,
     is_supersonic,
     supersonic_time,
     handbrake_val,
     is_auto_flipping,
@@ -681,14 +683,21 @@
         }
     }
 }
 
 impl GameState {
     pub const MIN_NUM_BYTES: usize = u64::NUM_BYTES + f32::NUM_BYTES + 1 + u32::NUM_BYTES * 2;
 
+    fn count_bytes(&self) -> usize {
+        Self::MIN_NUM_BYTES
+            + BallState::NUM_BYTES
+            + self.pads.len() * BoostPad::NUM_BYTES
+            + self.cars.len() * CarInfo::NUM_BYTES
+    }
+
     #[inline]
     pub fn get_num_bytes(bytes: &[u8]) -> usize {
         Self::MIN_NUM_BYTES
             + BallState::NUM_BYTES
             + Self::read_num_pads(bytes) * BoostPad::NUM_BYTES
             + Self::read_num_cars(bytes) * CarInfo::NUM_BYTES
     }
@@ -701,15 +710,15 @@
     #[inline]
     pub fn read_tick_rate(bytes: &[u8]) -> f32 {
         f32::from_bytes(&bytes[u64::NUM_BYTES..u64::NUM_BYTES + f32::NUM_BYTES])
     }
 
     #[inline]
     pub fn read_game_mode(bytes: &[u8]) -> GameMode {
-        GameMode::from_bytes(&bytes[u64::NUM_BYTES + f32::NUM_BYTES..u64::NUM_BYTES + f32::NUM_BYTES + 1])
+        GameMode::from_bytes(&bytes[(u64::NUM_BYTES + f32::NUM_BYTES)..=(u64::NUM_BYTES + f32::NUM_BYTES)])
     }
 
     #[inline]
     pub fn read_num_pads(bytes: &[u8]) -> usize {
         u32::from_bytes(&bytes[u64::NUM_BYTES + f32::NUM_BYTES + 1..u64::NUM_BYTES + f32::NUM_BYTES + 1 + u32::NUM_BYTES])
             as usize
     }
@@ -722,20 +731,15 @@
 
 pub trait ToBytes {
     fn to_bytes(&self) -> Vec<u8>;
 }
 
 impl ToBytes for GameState {
     fn to_bytes(&self) -> Vec<u8> {
-        let mut bytes = Vec::with_capacity(
-            Self::MIN_NUM_BYTES
-                + BallState::NUM_BYTES
-                + self.pads.len() * BoostPad::NUM_BYTES
-                + self.cars.len() * CarInfo::NUM_BYTES,
-        );
+        let mut bytes = Vec::with_capacity(self.count_bytes());
 
         bytes.extend(self.tick_count.to_bytes());
         bytes.extend(self.tick_rate.to_bytes());
         bytes.extend(self.game_mode.to_bytes());
         bytes.extend(&(self.pads.len() as u32).to_bytes());
         bytes.extend(&(self.cars.len() as u32).to_bytes());
         bytes.extend(self.ball.to_bytes());
```

### Comparing `rlviser_py-0.6.6/src/lib.rs` & `rlviser_py-0.6.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.6/src/socket.rs` & `rlviser_py-0.6.7/src/socket.rs`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.6/Cargo.lock` & `rlviser_py-0.6.7/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
-version = "0.2.154"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "lock_api"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
@@ -90,17 +90,17 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.21.2"
@@ -180,15 +180,15 @@
 checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rlviser-py"
-version = "0.6.6"
+version = "0.6.7"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
@@ -199,17 +199,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.60"
+version = "2.0.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+checksum = "7ad3dee41f36859875573074334c200d1add8e4a87bb37113ebd31d926b7b11f"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `rlviser_py-0.6.6/PKG-INFO` & `rlviser_py-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rlviser-py
-Version: 0.6.6
+Version: 0.6.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python implementation that manages a UDP connection to RLViser
 Keywords: rlviser,rocket-league,udp,python,rlbot
 License: MIT
```

