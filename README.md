# oneplus_8e_slim_hmbird
Buildin slim and hmbird_sched_proc By schqiushui &lt;orochi9999@gmail.com>
- [Commit edd6104](https://github.com/schqiushui/android_kernel_common_oneplus_sm8750/commit/edd6104ae623b53326af6929d92153b68bdc24cd)
- Patch **kernel/sched/build_policy.c**

```patch
 #ifdef CONFIG_SCHED_CLASS_EXTAdd commentMore actions
 # include "ext.c"
+# include "hmbird_sched_proc_main.c"
+#endif
+
+#ifdef CONFIG_SLIM_SCHED
+# include "slim_sysctl.c"
 #endif
```
- Maybe [Commit 822fe36](https://github.com/schqiushui/android_kernel_common_oneplus_sm8750/commit/822fe366af87e113983b3e0b7b823c2c7eb4ddf4) also helps