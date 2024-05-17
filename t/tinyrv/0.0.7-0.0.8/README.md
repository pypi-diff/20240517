# Comparing `tmp/tinyrv-0.0.7.tar.gz` & `tmp/tinyrv-0.0.8.tar.gz`

## Comparing `tinyrv-0.0.7.tar` & `tinyrv-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,35 @@
--rwxr-xr-x   0        0        0     3225 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tinyrv_opcodes_gen.py
--rw-r--r--   0        0        0  1095617 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/Image.gz
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/config.ini
--rwxr-xr-x   0        0        0     3337 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/linux.py
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/run_riscof.sh
--rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/run_riscv_tests.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/sixtyfourmb.dtb
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/sixtyfourmb.dts
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/sail_cSim/__init__.py
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/sail_cSim/riscof_sail_cSim.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/sail_cSim/env/link.ld
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/sail_cSim/env/model_test.h
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/tinyrv/riscof_tinyrv.py
--rwxr-xr-x   0        0        0      876 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/tinyrv/runner.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/tinyrv/tinyrv_isa.yaml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/tinyrv/tinyrv_platform.yaml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/tinyrv/env/link.ld
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tests/tinyrv/env/model_test.h
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tinyrv/__init__.py
--rw-r--r--   0        0        0   392314 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tinyrv/opcodes.py
--rw-r--r--   0        0        0    23217 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tinyrv/tinyrv.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tinyrv/tinyrv_dump.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 tinyrv-0.0.7/tinyrv/tinyrv_sim.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 tinyrv-0.0.7/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tinyrv-0.0.7/LICENSE
--rw-r--r--   0        0        0     8790 2020-02-02 00:00:00.000000 tinyrv-0.0.7/README.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 tinyrv-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     9285 2020-02-02 00:00:00.000000 tinyrv-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0     4150 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tinyrv_opcodes_gen.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/Makefile
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/mini.c
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/riscof_config32.ini
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/riscof_config64.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/br2_external_tinyrv/Config.in
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/br2_external_tinyrv/external.desc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/br2_external_tinyrv/external.mk
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/br2_external_tinyrv/board/tinyrv/linux.config
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/br2_external_tinyrv/configs/tinyrv_defconfig
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/coremark_tinyrv_port/core_portme.c
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/coremark_tinyrv_port/core_portme.h
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/coremark_tinyrv_port/core_portme.mak
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/sail_cSim/__init__.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/sail_cSim/riscof_sail_cSim.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/sail_cSim/env/link.ld
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/sail_cSim/env/model_test.h
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/tinyrv/riscof_tinyrv.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/tinyrv/tinyrv_isa32.yaml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/tinyrv/tinyrv_isa64.yaml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/tinyrv/tinyrv_platform.yaml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/tinyrv/env/link.ld
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tests/tinyrv/env/model_test.h
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tinyrv/__init__.py
+-rw-r--r--   0        0        0   537631 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tinyrv/opcodes.py
+-rwxr-xr-x   0        0        0    15943 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tinyrv/system.py
+-rw-r--r--   0        0        0    24260 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tinyrv/tinyrv.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tinyrv/tinyrv_dump.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tinyrv/tinyrv_sim.py
+-rw-r--r--   0        0        0    11998 2020-02-02 00:00:00.000000 tinyrv-0.0.8/tinyrv/vm.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 tinyrv-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tinyrv-0.0.8/LICENSE
+-rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 tinyrv-0.0.8/README.md
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 tinyrv-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 tinyrv-0.0.8/PKG-INFO
```

### Comparing `tinyrv-0.0.7/tinyrv_opcodes_gen.py` & `tinyrv-0.0.8/tinyrv_opcodes_gen.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,30 +22,44 @@
     del op['encoding']
     op['arg_bits'] = {}
     for vf in op['variable_fields']:
         if vf not in arg_bits: continue
         bits = [-1] * (32-len(arg_bits[vf])) + arg_bits[vf]  # padding for proper alignment when combining hi and lo fields
         vf2 = vf.replace('hi','').replace('lo','').replace('c_','')
         op['arg_bits'][vf2] = [max(a,b) for a, b in zip(op['arg_bits'][vf2], bits)] if vf2 in op['arg_bits'] else bits
-    for vf in op['arg_bits']: op['arg_bits'][vf] = op['arg_bits'][vf][next(n for n, e in enumerate(op['arg_bits'][vf]) if e >= 0):]  # remove padding
+    op['arg_getter'] = {}
+    for vf in op['arg_bits']:
+        op['arg_bits'][vf] = op['arg_bits'][vf][next(n for n, e in enumerate(op['arg_bits'][vf]) if e >= 0):]  # remove padding
+        pieces, prev_shift, prev_mask = [], None, None
+        for target, source in enumerate(op['arg_bits'][vf][::-1]):
+            if source < 0: continue
+            shift = f'>>{source-target}' if target < source else f'<<{target-source}' if target > source else ''
+            if shift == prev_shift:
+                prev_mask |= 1<<target
+                pieces[-1] = f'(x{shift})&{prev_mask}'
+            else:
+                prev_shift, prev_mask = shift, 1<<target
+                pieces.append(f'(x{shift})&{1<<target}')
+            op['arg_getter'][vf] = f'$sext({len(op["arg_bits"][vf])},' + '|'.join(pieces) + ')$' if op['arg_bits'][vf][0] == 31 and vf != 'csr' else '$' + '|'.join(pieces) + '$'
 
 common_ops = ('addi,sw,lw,jal,bne,beq,add,jalr,lbu,slli,lui,andi,or,bltu,srli,and,sub,blt,bgeu,xor,sb,auipc,sltiu,bge,lb,mul,sltu,lhu,sll,srl,sh,amoadd_w,xori,ori,csrrci,csrrs,srai,fence,lr_w,sc_w,mulhu,amoor_w,lh,amoand_w,csrrsi,divu,div,remu,sra,slt,csrrw,amoswap_w,csrrc,mulh,fence_i,rem,mret,csrrwi').split(',')
-
 mask_match = []
 mask_match_aliases = collections.defaultdict(set)
 for mask in dict((opcodes[op]['mask'],1) for op in common_ops + list(opcodes)):
     matches = {}
     for op in opcodes.values():
         if op['mask'] != mask or op['name'].endswith('_rv32'): continue
         if op['match'] in matches: mask_match_aliases[matches[op['match']][1:-1]].add(op['name'])
         else: matches[op['match']] = f'${op["name"]}$'
     mask_match.append((mask, matches))
 
 print('writing tinyrv/opcodes.py')
 with open('tinyrv/opcodes.py', 'w') as f:
     f.write(f'# auto-generated by tinyrv_opcodes_gen.py\n')
-    f.write(f'opcodes={str(opcodes)}\n')
+    f.write('def sext(length, word): return word|~((1<<length)-1) if word&(1<<(length-1)) else word&((1<<length)-1)\n')
+    ostr = str(opcodes).replace("'$", "lambda x:").replace("$'", "")
+    f.write(f'opcodes={ostr}\n')
     f.write(f'arg_bits={str(arg_bits)}\n')
     f.write(f'csrs={str(csrs)}\n')
     dstr = str(mask_match).replace("'$", "opcodes['").replace("$'", "']")
     f.write(f'mask_match={dstr}\n')
     f.write(f'mask_match_aliases={dict(mask_match_aliases)}\n')
```

### Comparing `tinyrv-0.0.7/tests/sail_cSim/riscof_sail_cSim.py` & `tinyrv-0.0.8/tests/sail_cSim/riscof_sail_cSim.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         for entry in config:
             logger.debug(entry+' : '+config[entry])
         return sclass
 
     def initialise(self, suite, work_dir, archtest_env):
         self.suite = suite
         self.work_dir = work_dir
-        self.objdump_cmd = 'riscv{1}-unknown-elf-objdump -D {0} > {2};'
-        self.compile_cmd = 'riscv{1}-unknown-elf-gcc -march={0} \
+        self.objdump_cmd = 'riscv64-unknown-elf-objdump -D {0} > {1};'
+        self.compile_cmd = 'riscv64-unknown-elf-gcc -march={0} \
          -static -mcmodel=medany -fvisibility=hidden -nostdlib -nostartfiles\
          -T '+self.pluginpath+'/env/link.ld\
          -I '+self.pluginpath+'/env/\
          -I ' + archtest_env
 
     def build(self, isa_yaml, platform_yaml):
         ispec = utils.load_yaml(isa_yaml)['hart0']
@@ -59,19 +59,19 @@
             self.isa += 'm'
         if "C" in ispec["ISA"]:
             self.isa += 'c'
         if "F" in ispec["ISA"]:
             self.isa += 'f'
         if "D" in ispec["ISA"]:
             self.isa += 'd'
-        objdump = "riscv{0}-unknown-elf-objdump".format(self.xlen)
+        objdump = "riscv64-unknown-elf-objdump"
         if shutil.which(objdump) is None:
             logger.error(objdump+": executable not found. Please check environment setup.")
             raise SystemExit(1)
-        compiler = "riscv{0}-unknown-elf-gcc".format(self.xlen)
+        compiler = "riscv64-unknown-elf-gcc"
         if shutil.which(compiler) is None:
             logger.error(compiler+": executable not found. Please check environment setup.")
             raise SystemExit(1)
         if shutil.which(self.sail_exe[self.xlen]) is None:
             logger.error(self.sail_exe[self.xlen]+ ": executable not found. Please check environment setup.")
             raise SystemExit(1)
         if shutil.which(self.make) is None:
@@ -90,19 +90,19 @@
             test_dir = testentry['work_dir']
             test_name = test.rsplit('/',1)[1][:-2]
 
             elf = 'ref.elf'
 
             execute = "@cd "+testentry['work_dir']+";"
 
-            cmd = self.compile_cmd.format(testentry['isa'].lower(), self.xlen) + ' ' + test + ' -o ' + elf
+            cmd = self.compile_cmd.format(testentry['isa'].lower()) + ' ' + test + ' -o ' + elf
             compile_cmd = cmd + ' -D' + " -D".join(testentry['macros'])
             execute+=compile_cmd+";"
 
-            execute += self.objdump_cmd.format(elf, self.xlen, 'ref.disass')
+            execute += self.objdump_cmd.format(elf, 'ref.disass')
             sig_file = os.path.join(test_dir, self.name[:-1] + ".signature")
 
             execute += self.sail_exe[self.xlen] + ' --test-signature={0} {1} > {2}.log 2>&1;'.format(sig_file, elf, test_name)
 
             cov_str = ' '
             for label in testentry['coverage_labels']:
                 cov_str+=' -l '+label
```

### Comparing `tinyrv-0.0.7/tests/sail_cSim/env/model_test.h` & `tinyrv-0.0.8/tests/sail_cSim/env/model_test.h`

 * *Files identical despite different names*

### Comparing `tinyrv-0.0.7/tests/tinyrv/riscof_tinyrv.py` & `tinyrv-0.0.8/tests/tinyrv/riscof_tinyrv.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,52 +10,54 @@
     __model__ = "tinyrv"
     __version__ = "latest"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         config = kwargs['config']
         self.pluginpath=os.path.abspath(config['pluginpath'])
-        self.dut_exe = "python3 " + os.path.join(self.pluginpath, "runner.py")
+        #self.dut_exe = "python3 " + os.path.join(self.pluginpath, "runner.py")
+        self.dut_exe = "tinyrv-vm-riscof"
         self.num_jobs = str(config.get('jobs', 1))
         self.isa_spec = os.path.abspath(config['ispec'])
         self.platform_spec = os.path.abspath(config['pspec'])
         self.target_run = config.get('target_run', '1') != '0'
 
     def initialise(self, suite, work_dir, archtest_env):
        self.work_dir = work_dir
        self.suite_dir = suite
-       self.compile_cmd = 'riscv{1}-unknown-elf-gcc -march={0} \
+       self.compile_cmd = 'riscv64-unknown-elf-gcc -march={0} \
          -static -mcmodel=medany -fvisibility=hidden -nostdlib -nostartfiles -g\
          -T '+self.pluginpath+'/env/link.ld\
          -I '+self.pluginpath+'/env/\
-         -I ' + archtest_env + ' {2} -o {3} {4}'
+         -I ' + archtest_env + ' {1} -o {2} {3}'
 
     def build(self, isa_yaml, platform_yaml):
       ispec = utils.load_yaml(isa_yaml)['hart0']
       self.xlen = ('64' if 64 in ispec['supported_xlen'] else '32')
       self.compile_cmd = self.compile_cmd+' -mabi='+('lp64 ' if 64 in ispec['supported_xlen'] else 'ilp32 ')
 
     def runTests(self, testList):
 
       # Delete Makefile if it already exists.
       if os.path.exists(self.work_dir+ "/Makefile." + self.name[:-1]):
             os.remove(self.work_dir+ "/Makefile." + self.name[:-1])
-      
+
       make = utils.makeUtil(makefilePath=os.path.join(self.work_dir, "Makefile." + self.name[:-1]))
       make.makeCommand = 'make -k -j' + self.num_jobs
 
       for testname in testList:
           testentry = testList[testname]
           test = testentry['test_path']
           test_dir = testentry['work_dir']
           elf = 'my.elf'
           compile_macros= ' -D' + " -D".join(testentry['macros'])
-          cmd = self.compile_cmd.format(testentry['isa'].lower(), self.xlen, test, elf, compile_macros)
+          cmd = self.compile_cmd.format(testentry['isa'].lower(), test, elf, compile_macros)
           if self.target_run:
-            simcmd = self.dut_exe + (' 64' if '64' in testentry['isa'] else ' 32')
+            #simcmd = self.dut_exe + (' 64' if '64' in testentry['isa'] else ' 32')
+            simcmd = self.dut_exe + ' my.elf >DUT-tinyrv.signature'
           else:
             simcmd = 'echo "NO RUN"'
 
           execute = '@cd {0}; {1}; {2};'.format(testentry['work_dir'], cmd, simcmd)
           make.add_target(execute)
 
       make.execute_all(self.work_dir)
```

### Comparing `tinyrv-0.0.7/tests/tinyrv/env/model_test.h` & `tinyrv-0.0.8/tests/tinyrv/env/model_test.h`

 * *Files identical despite different names*

### Comparing `tinyrv-0.0.7/tinyrv/tinyrv.py` & `tinyrv-0.0.8/tinyrv/tinyrv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, struct, array, struct
+import os, struct, array, struct, collections, functools
 from .opcodes import *
 
 iregs = 'zero,ra,sp,gp,tp,t0,t1,t2,fp,s1,a0,a1,a2,a3,a4,a5,a6,a7,s2,s3,s4,s5,s6,s7,s8,s9,s10,s11,t3,t4,t5,t6'.split(',')
 customs={0b0001011: 'custom0', 0b0101011: 'custom1', 0b1011011: 'custom2', 0b1111011: 'custom3'}
 def zext(length, word): return word&((1<<length)-1)
 def sext(length, word): return word|~((1<<length)-1) if word&(1<<(length-1)) else zext(length, word)
 def xfmt(length, word): return f'{{:0{length//4}x}}'.format(zext(length, word))
@@ -24,70 +24,77 @@
 
 def rvsplitter(*data, base=0, lower16=0):  # yields addresses and 32-bit/16-bit(compressed) RISC-V instruction words.
     for addr, instr in enumerate(struct.iter_unpack('<H', open(data[0],'rb').read() if isinstance(data[0],str) and os.path.isfile(data[0]) else array.array('I',[int(d,16) if isinstance(d,str) else d for d in (data[0] if hasattr(data[0], '__iter__') and not isinstance(data[0],str) else data)]))):
         if lower16: yield int(base)+(addr-1)*2, (instr[0]<<16)|lower16; lower16 = 0
         elif instr[0]&3 == 3: lower16 = instr[0]  # Two LSBs set: 32-bit instruction
         else: yield int(base)+addr*2, instr[0]
 
+@functools.lru_cache(maxsize=4096)
 def decode(instr, addr=0):  # decodes one instruction
     o = rvop(addr=addr, data=instr, name=customs.get(instr&0b1111111,'UNKNOWN'), args={})
     for mask, m_dict in mask_match:
         if op := m_dict.get(instr&mask, None):
-            for vf, bits in op['arg_bits'].items():
-                value = 0
-                for bit in bits: value = (value<<1) | ((instr>>bit)&1 if bit>=0 else 0)
-                o.args[vf] = sext(len(bits), value) if bits[0] == 31 else value
+            o.args = dict((vf, getter(instr)) for vf, getter in op['arg_getter'].items())
             [setattr(o,k,v) for k,v in (op|o.args).items()]
             break
     return o
 
 def decoder(*data, base=0):  # yields decoded instructions.
     for addr, instr in rvsplitter(*data, base=base):
         if instr != 0: yield decode(instr, addr)
 
 class sim:  # simulates RV32IMAZicsr_Zifencei, RV64IMAZicsr_Zifencei
     class rvregs:
         def __init__(self, xlen, sim): self._x, self.xlen, self.sim = [0]*32, xlen, sim
         def __getitem__(self, i): return self._x[i]
         def __setitem__(self, i, d):
-            if i!=0 and (self.sim.trace_log is not None) and d!=self._x[i]: self.sim.trace_log.append(f'{iregs[i]}=' + (f'{zext(self.xlen, d):08x}' if d>>32 in (0, -1) else f'{zext(self.xlen, d):016x}'))
+            if i!=0 and (self.sim.trace_log is not None) and d!=self._x[i]: self.sim.trace_log.append(f'{iregs[i]}=' + (f'{zext(self.xlen, d):08x}' if self.xlen==32 else f'{zext(self.xlen, d):016x}'))
             if i!=0: self._x[i] = d
+        def __repr__(self): return '\n'.join(['  '.join([f'x{r+rr:02d}({(iregs[r+rr])[-2:]})={xfmt(self.xlen, self._x[r+rr])}' for r in range(0, 32, 8)]) for rr in range(8)])
     def __init__(self, xlen=64, trap_misaligned=True):
         self.xlen, self.trap_misaligned, self.trace_log = xlen, trap_misaligned, []
-        self.pc, self.x, self.f, self.csr, self.lr_res_addr, self.cycle, self.current_mode, self.mem_psize, self.mem_pages, self.fmt_conv = 0, self.rvregs(self.xlen, self), [0]*32, [0]*4096, -1, 0, 3, 2<<12, {}, {'q': 64, 'Q': 64, 'i': 32, 'I': 32, 'h': 16, 'H': 16, 'b': 8, 'B': 8, 32: 'i', 64: 'q'}
-        [setattr(self, n, i) for i, n in list(enumerate(iregs))+list(csrs.items())]  # convenience
-    def __repr__(self): return '\n'.join(['  '.join([f'x{r+rr:02d}({(iregs[r+rr])[-2:]})={xfmt(self.xlen, self.x[r+rr])}' for r in range(0, 32, 8)]) for rr in range(8)])
+        self.pc, self.x, self.f, self.csr, self.lr_res_addr, self.cycle, self.current_mode, self.mem_psize, self.mem_pages = 0, self.rvregs(self.xlen, self), [0]*32, [0]*4096, -1, 0, 3, 2<<20, collections.defaultdict(functools.partial(bytearray, 2<<20))
+        [setattr(self, n, i) for i, n in list(enumerate(iregs))]; [setattr(self, 'csr_'+n, i) for i, n in list(csrs.items())]  # convenience
     def hook_csr(self, csr, reqval): return reqval if (csr&0xc00)!=0xc00 else self.csr[csr]
     def notify_stored(self, addr): pass  # called *after* mem store
     def notify_loading(self, addr): pass  # called *before* mem load
     def mtrap(self, tval, cause):
-        self.csr[self.mtval], self.csr[self.mepc], self.csr[self.mcause], self.pc = zext(self.xlen,tval), self.op.addr, cause, zext(self.xlen,self.csr[self.mtvec]&(~3))
-        if self.trace_log is not None: self.trace_log.append(f'mtrap cause={hex(cause)} tval={hex(tval)}')
-        self.csr[self.mstatus] = ((self.csr[self.mstatus]&0x08) << 4) | (self.current_mode << 11)
-    def read_bin(self, file, base=0): [self.store('B', i+base, b, notify=False) for i, b in enumerate(open(file, 'rb').read())]  # FIXME: SLOOOOW
-    def page_and_offset(self, addr):
-        if addr&~(self.mem_psize-1) not in self.mem_pages: self.mem_pages[addr&~(self.mem_psize-1)] = bytearray(self.mem_psize)
-        return self.mem_pages[addr&~(self.mem_psize-1)], addr&(self.mem_psize-1)
+        self.csr[self.csr_mtval], self.csr[self.csr_mepc], self.csr[self.csr_mcause], self.pc = zext(self.xlen,tval), self.op.addr, cause, zext(self.xlen,self.csr[self.csr_mtvec]&(~3))  # TODO: vectored interrupts
+        if self.trace_log is not None: self.trace_log.append(f'mtrap from_mode={self.current_mode} cause={hex(cause)} tval={hex(tval)}')
+        self.csr[self.csr_mstatus], self.current_mode = ((self.csr[self.csr_mstatus]&0x08) << 4) | (self.current_mode << 11), 3
+    def page_and_offset_iter(self, addr, nbytes):
+        while nbytes > 0:
+            page, poffset = self.page_and_offset(zext(self.xlen, addr))
+            yield page, poffset, (current := min(nbytes, self.mem_psize - poffset))
+            addr, nbytes = addr+current, nbytes-current
+    def copy_in(self, addr, bytes, doffset=0):
+        for page, offset, chunk in self.page_and_offset_iter(addr, len(bytes)): page[offset:offset+chunk] = bytes[doffset:(doffset:=doffset+chunk)]
+    def copy_out(self, addr, nbytes, doffset=0):
+        data = bytearray(nbytes+doffset)
+        for page, offset, chunk in self.page_and_offset_iter(addr, nbytes): data[doffset:(doffset:=doffset+chunk)] = page[offset:offset+chunk]
+        return data
+    def page_and_offset(self, addr): return self.mem_pages[addr&~(self.mem_psize-1)], addr&(self.mem_psize-1)
     def store(self, format, addr, data, notify=True):
         if self.trace_log is not None: self.trace_log.append(f'{xfmt(struct.calcsize(format)*8, data)}->mem[{xfmt(self.xlen, addr)}]')
         if self.trap_misaligned and addr&(struct.calcsize(format)-1) != 0: self.mtrap(addr, 6)
         else: struct.pack_into(format, *self.page_and_offset(zext(self.xlen,addr)), data)
         if notify: self.notify_stored(zext(self.xlen,addr))
-    def load(self, format, addr, fallback=0, notify=True, check_misaligned=True):
-        if check_misaligned and self.trap_misaligned and addr&(struct.calcsize(format)-1) != 0: self.mtrap(addr, 4); return fallback
-        if notify: self.notify_loading(zext(self.xlen,addr))
-        data = struct.unpack_from(format, *self.page_and_offset(zext(self.xlen,addr)))[0]
+    def load(self, format, addr, fallback=0, notify=True):
+        if self.trap_misaligned and addr&(struct.calcsize(format)-1) != 0: self.mtrap(addr, 4); return fallback
+        addr = zext(self.xlen, addr)
+        if notify: self.notify_loading(addr)
+        data = struct.unpack_from(format, *self.page_and_offset(addr))[0]
         if self.trace_log is not None: self.trace_log.append(f'mem[{xfmt(self.xlen, addr)}]->{xfmt(struct.calcsize(format)*8, data)}')
         return data
     def idiv2zero(self, a, b): return -(-a // b) if (a < 0) ^ (b < 0) else a // b
     def rem2zero(self, a, b): return a - b * self.idiv2zero(a, b)
     def _auipc    (self, rd, imm20,        **_): self.pc+=4; self.x[rd] = sext(self.xlen, self.op.addr+imm20)
     def _lui      (self, rd, imm20,        **_): self.pc+=4; self.x[rd] = imm20
-    def _jal      (self, rd, jimm20,       **_): self.pc, self.x[rd] = zext(self.xlen, self.op.addr+jimm20),    self.op.addr+4
-    def _jalr     (self, rd, rs1, imm12,   **_): self.pc, self.x[rd] = zext(self.xlen, self.x[rs1]+imm12)&(~1), self.op.addr+4 # LSB=0
+    def _jal      (self, rd, jimm20,       **_): self.pc, self.x[rd] = zext(self.xlen, self.op.addr+jimm20),    sext(self.xlen, self.op.addr+4)
+    def _jalr     (self, rd, rs1, imm12,   **_): self.pc, self.x[rd] = zext(self.xlen, self.x[rs1]+imm12)&(~1), sext(self.xlen, self.op.addr+4) # LSB=0
     def _beq      (self, rs1, rs2, bimm12, **_): self.pc = (self.op.addr+bimm12) if self.x[rs1] == self.x[rs2] else self.op.addr+4
     def _bne      (self, rs1, rs2, bimm12, **_): self.pc = (self.op.addr+bimm12) if self.x[rs1] != self.x[rs2] else self.op.addr+4
     def _blt      (self, rs1, rs2, bimm12, **_): self.pc = (self.op.addr+bimm12) if self.x[rs1] <  self.x[rs2] else self.op.addr+4
     def _bge      (self, rs1, rs2, bimm12, **_): self.pc = (self.op.addr+bimm12) if self.x[rs1] >= self.x[rs2] else self.op.addr+4
     def _bltu     (self, rs1, rs2, bimm12, **_): self.pc = (self.op.addr+bimm12) if zext(self.xlen, self.x[rs1]) <  zext(self.xlen, self.x[rs2]) else self.op.addr+4
     def _bgeu     (self, rs1, rs2, bimm12, **_): self.pc = (self.op.addr+bimm12) if zext(self.xlen, self.x[rs1]) >= zext(self.xlen, self.x[rs2]) else self.op.addr+4
     def _sb       (self, rs1, rs2, imm12,  **_): self.pc+=4; self.store('B', self.x[rs1]+imm12, zext( 8,self.x[rs2]))
@@ -133,15 +140,15 @@
     def _fence_i  (self,                   **_): self.pc+=4
     def _csrrw    (self, rd, csr, rs1,     **_): self.pc+=4; self.x[rd], self.csr[csr] = self.csr[csr], self.hook_csr(csr, self.x[rs1]               )
     def _csrrs    (self, rd, csr, rs1,     **_): self.pc+=4; self.x[rd], self.csr[csr] = self.csr[csr], self.hook_csr(csr, self.csr[csr]| self.x[rs1])
     def _csrrc    (self, rd, csr, rs1,     **_): self.pc+=4; self.x[rd], self.csr[csr] = self.csr[csr], self.hook_csr(csr, self.csr[csr]&~self.x[rs1])
     def _csrrwi   (self, rd, csr, zimm,    **_): self.pc+=4; self.x[rd], self.csr[csr] = self.csr[csr], self.hook_csr(csr, zimm                      )
     def _csrrsi   (self, rd, csr, zimm,    **_): self.pc+=4; self.x[rd], self.csr[csr] = self.csr[csr], self.hook_csr(csr, self.csr[csr]| zimm       )
     def _csrrci   (self, rd, csr, zimm,    **_): self.pc+=4; self.x[rd], self.csr[csr] = self.csr[csr], self.hook_csr(csr, self.csr[csr]&~zimm       )
-    def _mret     (self,                   **_): self.pc = zext(self.xlen, self.csr[self.mepc]); mmode = (self.csr[self.mstatus]>>11)&3; self.csr[self.mstatus] = (self.current_mode << 11) | 0x80 | ((self.csr[self.mstatus]&0x80) >> 4); self.current_mode = mmode
+    def _mret     (self,                   **_): self.pc = zext(self.xlen, self.csr[self.csr_mepc]); mmode = (self.csr[self.csr_mstatus]>>11)&3; self.csr[self.csr_mstatus] = (self.current_mode << 11) | 0x80 | ((self.csr[self.csr_mstatus]&0x80) >> 4); self.current_mode = mmode
     def _ecall    (self,                   **_): self.mtrap(0, 8 if self.current_mode == 0 else 11)
     def _ebreak   (self,                   **_): self.mtrap(self.op.addr, 3)
     def _mul      (self, rd, rs1, rs2,     **_): self.pc+=4; self.x[rd] = sext(self.xlen, (                self.x[rs1]  *                 self.x[rs2] )           )
     def _mulh     (self, rd, rs1, rs2,     **_): self.pc+=4; self.x[rd] = sext(self.xlen, (                self.x[rs1]  *                 self.x[rs2] )>>self.xlen)
     def _mulhu    (self, rd, rs1, rs2,     **_): self.pc+=4; self.x[rd] = sext(self.xlen, (zext(self.xlen, self.x[rs1]) * zext(self.xlen, self.x[rs2]))>>self.xlen)
     def _mulhsu   (self, rd, rs1, rs2,     **_): self.pc+=4; self.x[rd] = sext(self.xlen, (                self.x[rs1]  * zext(self.xlen, self.x[rs2]))>>self.xlen)
     def _div      (self, rd, rs1, rs2,     **_): self.pc+=4; self.x[rd] = sext(self.xlen, (self.idiv2zero( self.x[rs1]  ,                 self.x[rs2]))           ) if self.x[rs2] != 0 else -1
@@ -171,22 +178,26 @@
     def _amomin_d (self, rd, rs1, rs2,     **_): self.pc+=4; ors1, ors2 = self.x[rs1], self.x[rs2]; tmp = self.load('q', self.x[rs1], self.x[rd]); self.store('q', ors1, sext(64, min(        tmp , sext(64,ors2)))); self.x[rd]=tmp
     def _amomaxu_d(self, rd, rs1, rs2,     **_): self.pc+=4; ors1, ors2 = self.x[rs1], self.x[rs2]; tmp = self.load('q', self.x[rs1], self.x[rd]); self.store('q', ors1, sext(64, max(zext(64,tmp), zext(64,ors2)))); self.x[rd]=tmp
     def _amominu_d(self, rd, rs1, rs2,     **_): self.pc+=4; ors1, ors2 = self.x[rs1], self.x[rs2]; tmp = self.load('q', self.x[rs1], self.x[rd]); self.store('q', ors1, sext(64, min(zext(64,tmp), zext(64,ors2)))); self.x[rd]=tmp
     def _lr_w     (self, rd, rs1,          **_): self.pc+=4; self.lr_res_addr = self.x[rs1]; self.x[rd] = self.load('i', self.x[rs1], self.x[rd])
     def _sc_w     (self, rd, rs1, rs2,     **_):
         if self.lr_res_addr == self.x[rs1]: self.pc+=4; self.lr_res_addr = -1; self.store('i', self.x[rs1], sext(32, self.x[rs2])); self.x[rd] = 0
         else:                               self.pc+=4; self.lr_res_addr = -1;                                                      self.x[rd] = 1
+    def _lr_d     (self, rd, rs1,          **_): self.pc+=4; self.lr_res_addr = self.x[rs1]; self.x[rd] = self.load('q', self.x[rs1], self.x[rd])
+    def _sc_d     (self, rd, rs1, rs2,     **_):
+        if self.lr_res_addr == self.x[rs1]: self.pc+=4; self.lr_res_addr = -1; self.store('q', self.x[rs1], sext(64, self.x[rs2])); self.x[rd] = 0
+        else:                               self.pc+=4; self.lr_res_addr = -1;                                                      self.x[rd] = 1
     def _c_addi  (self, rd_rs1_n0, nzimm6, **_): self.pc+=2; self.x[rd_rs1_n0] += nzimm6  # c.nop required to pass test rv32i_m/privilege/src/misalign-jal-01.S
     def hook_exec(self): return True
     def unimplemented(self, **_): print(f'\n{zext(64,self.op.addr):08x}: unimplemented: {zext(32,self.op.data):08x} {self.op}')
     def step(self, trace=True):
-        self.op = decode(self.load('I', self.pc, notify=False, check_misaligned=False), addr=self.pc)
-        self.cycle += 1; self.csr[self.mcycle] = zext(self.xlen, self.cycle)
+        self.op = decode(struct.unpack_from('I', *self.page_and_offset(self.pc))[0]); self.op.addr=self.pc  # setting op.addr afterwards enables opcode caching.
         self.trace_log = [] if trace else None
         if self.hook_exec():
+            self.cycle += 1; self.csr[self.csr_mcycle] = zext(self.xlen, self.cycle)
             getattr(self, '_'+self.op.name, self.unimplemented)(**self.op.args)  # dynamic instruction dispatch
-            if trace: print(f'{zext(64,self.op.addr):08x}: {str(self.op):40} #', ' '.join(self.trace_log))
+            if trace: print(f'{zext(64,self.op.addr):08x}: {str(self.op):40} # [{self.cycle-1}]', ' '.join(self.trace_log))
             if trace and self.pc-self.op.addr not in (2, 4): print()
     def run(self, limit=0, bpts=set(), trace=True):
         while True:
             self.step(trace=trace)
             if self.op.addr in bpts|{self.pc} or (limit := limit-1)==0: break
```

### Comparing `tinyrv-0.0.7/tinyrv/tinyrv_sim.py` & `tinyrv-0.0.8/tinyrv/tinyrv_sim.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 
 def main():
     if len(sys.argv) < 2: print(f'usage: {pathlib.Path(sys.argv[0]).name} file.bin [(32|64) [run limit in decimal [start PC in hex]]]'); exit(1)
     xlen = 32 if len(sys.argv) < 3 else int(sys.argv[2])
     limit = 0 if len(sys.argv) < 4 else int(sys.argv[3])
     pc = 0 if len(sys.argv) < 5 else int(sys.argv[4], 16)
     rv = tinyrv.sim(xlen=xlen, trap_misaligned=False)
-    rv.read_bin(sys.argv[1], base=0)
+    rv.copy_in(0, open(sys.argv[1], 'rb').read())
     rv.pc = pc
     rv.run(limit)
 
 if __name__ == '__main__': main()
```

### Comparing `tinyrv-0.0.7/LICENSE` & `tinyrv-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyrv-0.0.7/README.md` & `tinyrv-0.0.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 {'rd': 2, 'rs1': 2, 'imm12': -220} 2 2 -220
 sp, sp, -220
 ```
 Simulate a binary:
 ```py
 rv = tinyrv.sim(xlen=32)  # xlen affects overflows, sign extensions
 rv.read_bin('firmware.bin', base=0)
-print(rv)  # print registers
+print(rv.x)  # print registers
 print()
 rv.step()  # simulate a single instruction at rv.pc
 ```
 Outputs:
 ```
 x00(ro)=00000000  x08(fp)=00000000  x16(a6)=00000000  x24(s8)=00000000
 x01(ra)=00000000  x09(s1)=00000000  x17(a7)=00000000  x25(s9)=00000000
@@ -163,24 +163,28 @@
 
 tinyrv-sim firmware.bin 32 100 8
 ```
 
 
 ## Dev Setup
 
-All code is in `tinyrv/tinyrv.py` and has no external dependencies.
-tinyRV loads opcode specs from `tinyrv/opcodes.py`, which is auto-generated by `tinyrv_opcodes_gen.py` from [riscv-opcodes](https://github.com/riscv/riscv-opcodes).
+All core simulator code is in `tinyrv/tinyrv.py` and has no external dependencies.
+tinyRV loads opcode specs from `tinyrv/opcodes.py`, which is auto-generated from [riscv-opcodes](https://github.com/riscv/riscv-opcodes) by `tinyrv_opcodes_gen.py`.
 
 Do this to re-generate:
-```sh
+```bash
 git clone https://github.com/riscv/riscv-opcodes.git
 make -C riscv-opcodes
 python3 tinyrv_opcodes_gen.py
 ```
 
+Some VMs use external libraries:
+- [lief](https://pypi.org/project/lief/) for loading ELFs
+- [readchar](https://pypi.org/project/readchar/) for reading keystrokes
+- [dataclasses-struct](https://pypi.org/project/dataclasses-struct/) for easier binary data manipulation
 
 ## Testing
 
 Install [riscv-gnu-toolchain](https://github.com/riscv/riscv-gnu-toolchain) or [homebrew-riscv](https://github.com/riscv-software-src/homebrew-riscv) (for MacOS).
 
 ### RISCOF
 
@@ -219,38 +223,47 @@
 ../configure --prefix=/path/to/install  # /path/to/install/bin must be in $PATH
 make
 make install
 spike  # test
 ```
 Then, run the tests:
 ```sh
-cd tests
-riscof --verbose info arch-test --clone
-./run_riscof.sh
+make -C tests run_riscof
 ```
 
+
 ### riscv-software-src/riscv-tests
 
 ```sh
-cd tests
-git clone https://github.com/riscv/riscv-tests
-cd riscv-tests
-git submodule update --init --recursive
-autoconf
-./configure
-make
-cd ..
-./run_riscv_tests.py
+make -C tests run_riscv_tests
 ```
+This will automatically clone and build the test suite if necessary.
+
+### Run Coremark
+
+```sh
+make -C tests run_coremark
+```
+This will automatically clone and build coremark if necessary.
 
 ### Boot Linux
 
+```bash
+make -C tests run_linux
 ```
-cd tests
-python3 linux.py
+Will download an Image and boot it.
+Boottime is about a minute on a reasonable fast machine and recent Python.
+
+The Image was made using [buildroot](https://buildroot.org).
+The configuration is based on qemu_riscv64_nommu_virt_defconfig with FPU, compressed instructions and other extensions turned off.
+
+To (re-)create this Image, run:
+```bash
+make -C tests Image
 ```
-Takes 3-4 minutes on a reasonable fast machine and recent python.
+This will download buildroot and build the kernel (takes some time).
+The build configuration is in tests/br2_external_tinyrv.
 
 ## Related
 
 - [TinyFive](https://github.com/OpenMachine-ai/tinyfive)
 - [mini-rv32ima](https://github.com/cnlohr/mini-rv32ima)
```

### Comparing `tinyrv-0.0.7/PKG-INFO` & `tinyrv-0.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.3
 Name: tinyrv
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tiny RISC-V instruction set simulator
 Project-URL: Homepage, https://github.com/s-holst/tinyrv
 Project-URL: Issues, https://github.com/s-holst/tinyrv/issues
 Author-email: Stefan Holst <mail@s-holst.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: dataclasses-struct
+Requires-Dist: lief
+Requires-Dist: readchar
 Description-Content-Type: text/markdown
 
 # tinyRV
 
 A RISC-V instruction decoder and instruction set simulator in less than 200 lines of python.
 
 **Mission**: Make the most useful RISC-V disassembler/simulator for understanding the ISA and reverse-engineering binaries with the least amount of easily extendable code. Simulation performance is secondary.
@@ -84,15 +87,15 @@
 {'rd': 2, 'rs1': 2, 'imm12': -220} 2 2 -220
 sp, sp, -220
 ```
 Simulate a binary:
 ```py
 rv = tinyrv.sim(xlen=32)  # xlen affects overflows, sign extensions
 rv.read_bin('firmware.bin', base=0)
-print(rv)  # print registers
+print(rv.x)  # print registers
 print()
 rv.step()  # simulate a single instruction at rv.pc
 ```
 Outputs:
 ```
 x00(ro)=00000000  x08(fp)=00000000  x16(a6)=00000000  x24(s8)=00000000
 x01(ra)=00000000  x09(s1)=00000000  x17(a7)=00000000  x25(s9)=00000000
@@ -177,24 +180,28 @@
 
 tinyrv-sim firmware.bin 32 100 8
 ```
 
 
 ## Dev Setup
 
-All code is in `tinyrv/tinyrv.py` and has no external dependencies.
-tinyRV loads opcode specs from `tinyrv/opcodes.py`, which is auto-generated by `tinyrv_opcodes_gen.py` from [riscv-opcodes](https://github.com/riscv/riscv-opcodes).
+All core simulator code is in `tinyrv/tinyrv.py` and has no external dependencies.
+tinyRV loads opcode specs from `tinyrv/opcodes.py`, which is auto-generated from [riscv-opcodes](https://github.com/riscv/riscv-opcodes) by `tinyrv_opcodes_gen.py`.
 
 Do this to re-generate:
-```sh
+```bash
 git clone https://github.com/riscv/riscv-opcodes.git
 make -C riscv-opcodes
 python3 tinyrv_opcodes_gen.py
 ```
 
+Some VMs use external libraries:
+- [lief](https://pypi.org/project/lief/) for loading ELFs
+- [readchar](https://pypi.org/project/readchar/) for reading keystrokes
+- [dataclasses-struct](https://pypi.org/project/dataclasses-struct/) for easier binary data manipulation
 
 ## Testing
 
 Install [riscv-gnu-toolchain](https://github.com/riscv/riscv-gnu-toolchain) or [homebrew-riscv](https://github.com/riscv-software-src/homebrew-riscv) (for MacOS).
 
 ### RISCOF
 
@@ -233,38 +240,47 @@
 ../configure --prefix=/path/to/install  # /path/to/install/bin must be in $PATH
 make
 make install
 spike  # test
 ```
 Then, run the tests:
 ```sh
-cd tests
-riscof --verbose info arch-test --clone
-./run_riscof.sh
+make -C tests run_riscof
 ```
 
+
 ### riscv-software-src/riscv-tests
 
 ```sh
-cd tests
-git clone https://github.com/riscv/riscv-tests
-cd riscv-tests
-git submodule update --init --recursive
-autoconf
-./configure
-make
-cd ..
-./run_riscv_tests.py
+make -C tests run_riscv_tests
 ```
+This will automatically clone and build the test suite if necessary.
+
+### Run Coremark
+
+```sh
+make -C tests run_coremark
+```
+This will automatically clone and build coremark if necessary.
 
 ### Boot Linux
 
+```bash
+make -C tests run_linux
 ```
-cd tests
-python3 linux.py
+Will download an Image and boot it.
+Boottime is about a minute on a reasonable fast machine and recent Python.
+
+The Image was made using [buildroot](https://buildroot.org).
+The configuration is based on qemu_riscv64_nommu_virt_defconfig with FPU, compressed instructions and other extensions turned off.
+
+To (re-)create this Image, run:
+```bash
+make -C tests Image
 ```
-Takes 3-4 minutes on a reasonable fast machine and recent python.
+This will download buildroot and build the kernel (takes some time).
+The build configuration is in tests/br2_external_tinyrv.
 
 ## Related
 
 - [TinyFive](https://github.com/OpenMachine-ai/tinyfive)
 - [mini-rv32ima](https://github.com/cnlohr/mini-rv32ima)
```

