* [Burst Documentation](index.md)
  * [Quick Start](docs/QuickStart.md)
    * [Compile a Job with the Burst compiler](docs/QuickStart.md#compile-a-job-with-the-burst-compiler)
    * [Jobs/Burst Menu](docs/QuickStart.md#jobs-burst-menu)
    * [Burst Inspector](docs/QuickStart.md#burst-inspector)
    * [Command-line Options](docs/QuickStart.md#command-line-options)
    * [Just-In-Time (JIT) vs Ahead-Of-Time (AOT) Compilation](docs/QuickStart.md#just-in-time-jit-vs-ahead-of-time-aot-compilation)
  * [C#/.NET Language Support](docs/CSharpLanguageSupport_Types.md)
    * [Supported .NET types](docs/CSharpLanguageSupport_Types.md#supported-net-types)
      * [Primitive types](docs/CSharpLanguageSupport_Types.md#primitive-types)
      * [Vector types](docs/CSharpLanguageSupport_Types.md#vector-types)
      * [Enum types](docs/CSharpLanguageSupport_Types.md#enum-types)
      * [Struct types](docs/CSharpLanguageSupport_Types.md#struct-types)
      * [Pointer types](docs/CSharpLanguageSupport_Types.md#pointer-types)
      * [Generic types](docs/CSharpLanguageSupport_Types.md#generic-types)
      * [Array types](docs/CSharpLanguageSupport_Types.md#array-types)
    * [Language Support](docs/CSharpLanguageSupport_Lang.md#language-support)
      * [Throw and Exceptions](docs/CSharpLanguageSupport_Lang.md#throw-and-exceptions)
      * [Partial support for strings and `Debug.Log`](docs/CSharpLanguageSupport_Lang.md#partial-support-for-strings-and-debuglog)
    * [Intrinsics](docs/CSharpLanguageSupport_Intrinsics.md#intrinsics)
      * [System.Math](docs/CSharpLanguageSupport_Intrinsics.md#systemmath)
      * [System.IntPtr](docs/CSharpLanguageSupport_Intrinsics.md#systemintptr)
      * [System.Threading.Interlocked](docs/CSharpLanguageSupport_Intrinsics.md#systemthreadinginterlocked)
      * [System.Threading.Thread](docs/CSharpLanguageSupport_Intrinsics.md#systemthreadingthread)
      * [System.Threading.Volatile](docs/CSharpLanguageSupport_Intrinsics.md#systemthreadingvolatile)
    * [Unity.Burst.Intrinsics](docs/CSharpLanguageSupport_BurstIntrinsics.md#unityburstintrinsics)
      * [Common](docs/CSharpLanguageSupport_BurstIntrinsics.md#common)
      * [Pause](docs/CSharpLanguageSupport_BurstIntrinsics.md#pause)
      * [Prefetch](docs/CSharpLanguageSupport_BurstIntrinsics.md#prefetch)
      * [umul128](docs/CSharpLanguageSupport_BurstIntrinsics.md#umul128)
      * [Processor specific SIMD extensions](docs/CSharpLanguageSupport_BurstIntrinsics.md#processor-specific-simd-extensions)
      * [`DllImport` and internal calls](docs/CSharpLanguageSupport_BurstIntrinsics.md#dllimport-and-internal-calls)
  * [Debugging and Profiling](docs/DebuggingAndProfiling.md)
    * [Managed Debugging](docs/DebuggingAndProfiling.md#managed-debugging)
    * [Native Debugging](docs/DebuggingAndProfiling.md#native-debugging)
  * [Advanced Usages](docs/AdvancedUsages.md)
    * [BurstDiscard attribute](docs/AdvancedUsages.md#burstdiscard-attribute)
    * [Synchronous Compilation](docs/AdvancedUsages.md#synchronous-compilation)
    * [Disable Safety Checks](docs/AdvancedUsages.md#disable-safety-checks)
    * [Function Pointers](docs/AdvancedUsages.md#function-pointers)
      * [Performance considerations](docs/AdvancedUsages.md#performance-considerations)
    * [Shared Static](docs/AdvancedUsages.md#shared-static)
    * [Dynamic dispatch based on runtime CPU features](docs/AdvancedUsages.md#dynamic-dispatch-based-on-runtime-cpu-features)
  * [Optimization Guidelines](docs/OptimizationGuidelines.md)
    * [Aliasing](docs/OptimizationGuidelines-Aliasing.md)
      * [The Problem](docs/OptimizationGuidelines-Aliasing.md#the-problem)
        * [No memory aliasing](docs/OptimizationGuidelines-Aliasing.md#no-memory-aliasing)
        * [No memory aliasing with the auto-vectorizer](docs/OptimizationGuidelines-Aliasing.md#no-memory-aliasing-with-the-auto-vectorizer)
        * [Memory aliasing](docs/OptimizationGuidelines-Aliasing.md#memory-aliasing)
        * [Memory aliasing with invalid vectorized code](docs/OptimizationGuidelines-Aliasing.md#memory-aliasing-with-invalid-vectorized-code)
        * [Example of Generated Code](docs/OptimizationGuidelines-Aliasing.md#example-of-generated-code)
      * [Burst and the JobSystem](docs/OptimizationGuidelines-Aliasing.md#burst-and-the-jobsystem)
      * [The NoAlias Attribute](docs/OptimizationGuidelines-Aliasing.md#the-noalias-attribute)
        * [NoAlias Function Paramater](docs/OptimizationGuidelines-Aliasing.md#noalias-function-parameter)
        * [NoAlias Struct Field](docs/OptimizationGuidelines-Aliasing.md#noalias-struct-field)
        * [NoAlias Struct](docs/OptimizationGuidelines-Aliasing.md#noalias-struct)
        * [NoAlias Function Return](docs/OptimizationGuidelines-Aliasing.md#noalias-function-return)
      * [Function Cloning for Better Aliasing Deduction](docs/OptimizationGuidelines-Aliasing.md#function-cloning-for-better-aliasing-deduction)
      * [Aliasing Checks](docs/OptimizationGuidelines-Aliasing.md#aliasing-checks)
    * [Loop Vectorization](docs/OptimizationGuidelines.md#loop-vectorization)
    * [Compiler Options](docs/OptimizationGuidelines.md#compiler-options)
      * [FloatPrecision](docs/OptimizationGuidelines.md#floatprecision)
        * [FloatPrecision.Low](docs/OptimizationGuidelines.md#floatprecisionlow)
      * [Compiler floating point math mode](docs/OptimizationGuidelines.md#compiler-floating-point-math-mode)
    * [Assume Intrinsics](docs/OptimizationGuidelines.md#assume-intrinsics)
    * [Unity Mathematics](docs/OptimizationGuidelines.md#unitymathematics)
    * [Generic Jobs](docs/OptimizationGuidelines.md#generic-jobs)
  * [Standalone Player support](docs/StandalonePlayerSupport.md)
    * [Usage](docs/StandalonePlayerSupport.md#usage)
    * [Burst AOT Settings](docs/StandalonePlayerSupport.md#burst-aot-settings)
    * [Burst AOT Requirements](docs/StandalonePlayerSupport.md#burst-aot-requirements)
      * [Desktop platforms with cross compilation enabled (the default behaviour)](docs/StandalonePlayerSupport.md#desktop-platforms-with-cross-compilation-enabled-the-default-behaviour)
      * [Other platforms and desktops when cross compilation is disabled)](docs/StandalonePlayerSupport.md#other-platforms-and-desktops-when-cross-compilation-is-disabled)
    * [Burst Targets](docs/StandalonePlayerSupport.md#burst-targets)
  * [Known issues](docs/KnownIssues.md)
    * [`DllImport`](docs/KnownIssues.md#known-issues-with-dllimport)
    * [Debugging/Profiling](docs/KnownIssues.md#known-issues-with-debuggingprofiling)
  * [Presentations](docs/Presentations.md)
