
.. _l-onnx-doccom.microsoft-LambOptimizer:

=============================
com.microsoft - LambOptimizer
=============================

.. contents::
    :local:


.. _l-onnx-opcom-microsoft-lamboptimizer-1:

LambOptimizer - 1 (com.microsoft)
=================================

**Version**

* **name**: `LambOptimizer (GitHub) <https://github.com/onnx/onnx/blob/main/docs/Operators.md#com.microsoft.LambOptimizer>`_
* **domain**: **com.microsoft**
* **since_version**: **1**
* **function**:
* **support_level**:
* **shape inference**:

This version of the operator has been available
**since version 1 of domain com.microsoft**.

**Summary**

**Attributes**

* **alpha**:
  Coefficient of previous gradient in running average. Default value is ``?``.
* **beta**:
  Coefficient of previous squared gradient in running average.The
  effective learning rate is computed by r = R / (1 + T *
  decay_factor). Default to 0 so that increasing update counts doesn't
  reduce the learning rate. Default value is ``?``.
* **do_bias_correction**:
  Compute unbiased 1st and 2nd momentums. Default value is ``?``.
* **epsilon**:
  Small scalar to avoid dividing by zero. Default value is ``?``.
* **lambda**:
  Regularization coefficient of 0.5 * lambda * ||X||_2^2. Default to
  0, which means no regularization. Default value is ``?``.
* **max_norm_clip**:
  clip threshold of gradients. Default value is ``?``.
* **ratio_max**:
  Upper bound on confidence ratio. Default value is ``?``.
* **ratio_min**:
  Lower bound on confidence ratio. Default value is ``?``.

**Inputs**

Between 0 and 5125 inputs.

* **update_signal** (optional, heterogeneous) - **T_BOOL**:
  This signal indicates if weight tensors should be updated.
* **loss_scale** (optional, heterogeneous) - **T2**:
  Loss scale for mixed precision training.
* **gradient_norm** (optional, heterogeneous) - **T_GRAD_NORM**:
  Norm of global gradient.
* **R** (optional, heterogeneous) - **T1**:
  The initial learning rate.
* **step** (optional, heterogeneous) - **TInt64**:
  One-based index of the current training iteration.
* **__group_0__weights** (optional) - **T2**:
  weights to optimize.
* **__group_0__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_0__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_0__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_0__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_2__weights** (optional) - **T2**:
  weights to optimize.
* **__group_2__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_2__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_2__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_2__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_3__weights** (optional) - **T2**:
  weights to optimize.
* **__group_3__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_3__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_3__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_3__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_4__weights** (optional) - **T2**:
  weights to optimize.
* **__group_4__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_4__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_4__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_4__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_5__weights** (optional) - **T2**:
  weights to optimize.
* **__group_5__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_5__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_5__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_5__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_6__weights** (optional) - **T2**:
  weights to optimize.
* **__group_6__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_6__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_6__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_6__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_7__weights** (optional) - **T2**:
  weights to optimize.
* **__group_7__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_7__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_7__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_7__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_8__weights** (optional) - **T2**:
  weights to optimize.
* **__group_8__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_8__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_8__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_8__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_9__weights** (optional) - **T2**:
  weights to optimize.
* **__group_9__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_9__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_9__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_9__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_10__weights** (optional) - **T2**:
  weights to optimize.
* **__group_10__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_10__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_10__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_10__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_11__weights** (optional) - **T2**:
  weights to optimize.
* **__group_11__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_11__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_11__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_11__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_12__weights** (optional) - **T2**:
  weights to optimize.
* **__group_12__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_12__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_12__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_12__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_13__weights** (optional) - **T2**:
  weights to optimize.
* **__group_13__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_13__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_13__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_13__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_14__weights** (optional) - **T2**:
  weights to optimize.
* **__group_14__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_14__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_14__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_14__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_15__weights** (optional) - **T2**:
  weights to optimize.
* **__group_15__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_15__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_15__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_15__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_16__weights** (optional) - **T2**:
  weights to optimize.
* **__group_16__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_16__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_16__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_16__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_17__weights** (optional) - **T2**:
  weights to optimize.
* **__group_17__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_17__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_17__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_17__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_18__weights** (optional) - **T2**:
  weights to optimize.
* **__group_18__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_18__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_18__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_18__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_19__weights** (optional) - **T2**:
  weights to optimize.
* **__group_19__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_19__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_19__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_19__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_20__weights** (optional) - **T2**:
  weights to optimize.
* **__group_20__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_20__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_20__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_20__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_21__weights** (optional) - **T2**:
  weights to optimize.
* **__group_21__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_21__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_21__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_21__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_22__weights** (optional) - **T2**:
  weights to optimize.
* **__group_22__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_22__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_22__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_22__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_23__weights** (optional) - **T2**:
  weights to optimize.
* **__group_23__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_23__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_23__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_23__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_24__weights** (optional) - **T2**:
  weights to optimize.
* **__group_24__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_24__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_24__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_24__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_25__weights** (optional) - **T2**:
  weights to optimize.
* **__group_25__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_25__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_25__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_25__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_26__weights** (optional) - **T2**:
  weights to optimize.
* **__group_26__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_26__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_26__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_26__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_27__weights** (optional) - **T2**:
  weights to optimize.
* **__group_27__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_27__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_27__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_27__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_28__weights** (optional) - **T2**:
  weights to optimize.
* **__group_28__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_28__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_28__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_28__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_29__weights** (optional) - **T2**:
  weights to optimize.
* **__group_29__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_29__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_29__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_29__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_30__weights** (optional) - **T2**:
  weights to optimize.
* **__group_30__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_30__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_30__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_30__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_31__weights** (optional) - **T2**:
  weights to optimize.
* **__group_31__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_31__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_31__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_31__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_32__weights** (optional) - **T2**:
  weights to optimize.
* **__group_32__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_32__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_32__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_32__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_33__weights** (optional) - **T2**:
  weights to optimize.
* **__group_33__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_33__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_33__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_33__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_34__weights** (optional) - **T2**:
  weights to optimize.
* **__group_34__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_34__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_34__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_34__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_35__weights** (optional) - **T2**:
  weights to optimize.
* **__group_35__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_35__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_35__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_35__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_36__weights** (optional) - **T2**:
  weights to optimize.
* **__group_36__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_36__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_36__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_36__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_37__weights** (optional) - **T2**:
  weights to optimize.
* **__group_37__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_37__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_37__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_37__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_38__weights** (optional) - **T2**:
  weights to optimize.
* **__group_38__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_38__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_38__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_38__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_39__weights** (optional) - **T2**:
  weights to optimize.
* **__group_39__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_39__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_39__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_39__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_40__weights** (optional) - **T2**:
  weights to optimize.
* **__group_40__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_40__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_40__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_40__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_41__weights** (optional) - **T2**:
  weights to optimize.
* **__group_41__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_41__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_41__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_41__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_42__weights** (optional) - **T2**:
  weights to optimize.
* **__group_42__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_42__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_42__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_42__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_43__weights** (optional) - **T2**:
  weights to optimize.
* **__group_43__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_43__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_43__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_43__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_44__weights** (optional) - **T2**:
  weights to optimize.
* **__group_44__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_44__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_44__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_44__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_45__weights** (optional) - **T2**:
  weights to optimize.
* **__group_45__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_45__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_45__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_45__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_46__weights** (optional) - **T2**:
  weights to optimize.
* **__group_46__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_46__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_46__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_46__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_47__weights** (optional) - **T2**:
  weights to optimize.
* **__group_47__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_47__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_47__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_47__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_48__weights** (optional) - **T2**:
  weights to optimize.
* **__group_48__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_48__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_48__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_48__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_49__weights** (optional) - **T2**:
  weights to optimize.
* **__group_49__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_49__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_49__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_49__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_50__weights** (optional) - **T2**:
  weights to optimize.
* **__group_50__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_50__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_50__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_50__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_51__weights** (optional) - **T2**:
  weights to optimize.
* **__group_51__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_51__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_51__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_51__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_52__weights** (optional) - **T2**:
  weights to optimize.
* **__group_52__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_52__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_52__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_52__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_53__weights** (optional) - **T2**:
  weights to optimize.
* **__group_53__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_53__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_53__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_53__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_54__weights** (optional) - **T2**:
  weights to optimize.
* **__group_54__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_54__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_54__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_54__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_55__weights** (optional) - **T2**:
  weights to optimize.
* **__group_55__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_55__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_55__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_55__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_56__weights** (optional) - **T2**:
  weights to optimize.
* **__group_56__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_56__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_56__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_56__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_57__weights** (optional) - **T2**:
  weights to optimize.
* **__group_57__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_57__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_57__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_57__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_58__weights** (optional) - **T2**:
  weights to optimize.
* **__group_58__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_58__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_58__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_58__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_59__weights** (optional) - **T2**:
  weights to optimize.
* **__group_59__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_59__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_59__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_59__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_60__weights** (optional) - **T2**:
  weights to optimize.
* **__group_60__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_60__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_60__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_60__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_61__weights** (optional) - **T2**:
  weights to optimize.
* **__group_61__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_61__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_61__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_61__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_62__weights** (optional) - **T2**:
  weights to optimize.
* **__group_62__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_62__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_62__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_62__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_63__weights** (optional) - **T2**:
  weights to optimize.
* **__group_63__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_63__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_63__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_63__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_64__weights** (optional) - **T2**:
  weights to optimize.
* **__group_64__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_64__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_64__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_64__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_65__weights** (optional) - **T2**:
  weights to optimize.
* **__group_65__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_65__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_65__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_65__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_66__weights** (optional) - **T2**:
  weights to optimize.
* **__group_66__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_66__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_66__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_66__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_67__weights** (optional) - **T2**:
  weights to optimize.
* **__group_67__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_67__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_67__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_67__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_68__weights** (optional) - **T2**:
  weights to optimize.
* **__group_68__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_68__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_68__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_68__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_69__weights** (optional) - **T2**:
  weights to optimize.
* **__group_69__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_69__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_69__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_69__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_70__weights** (optional) - **T2**:
  weights to optimize.
* **__group_70__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_70__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_70__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_70__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_71__weights** (optional) - **T2**:
  weights to optimize.
* **__group_71__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_71__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_71__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_71__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_72__weights** (optional) - **T2**:
  weights to optimize.
* **__group_72__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_72__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_72__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_72__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_73__weights** (optional) - **T2**:
  weights to optimize.
* **__group_73__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_73__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_73__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_73__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_74__weights** (optional) - **T2**:
  weights to optimize.
* **__group_74__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_74__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_74__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_74__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_75__weights** (optional) - **T2**:
  weights to optimize.
* **__group_75__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_75__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_75__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_75__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_76__weights** (optional) - **T2**:
  weights to optimize.
* **__group_76__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_76__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_76__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_76__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_77__weights** (optional) - **T2**:
  weights to optimize.
* **__group_77__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_77__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_77__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_77__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_78__weights** (optional) - **T2**:
  weights to optimize.
* **__group_78__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_78__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_78__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_78__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_79__weights** (optional) - **T2**:
  weights to optimize.
* **__group_79__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_79__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_79__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_79__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_80__weights** (optional) - **T2**:
  weights to optimize.
* **__group_80__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_80__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_80__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_80__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_81__weights** (optional) - **T2**:
  weights to optimize.
* **__group_81__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_81__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_81__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_81__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_82__weights** (optional) - **T2**:
  weights to optimize.
* **__group_82__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_82__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_82__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_82__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_83__weights** (optional) - **T2**:
  weights to optimize.
* **__group_83__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_83__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_83__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_83__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_84__weights** (optional) - **T2**:
  weights to optimize.
* **__group_84__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_84__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_84__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_84__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_85__weights** (optional) - **T2**:
  weights to optimize.
* **__group_85__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_85__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_85__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_85__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_86__weights** (optional) - **T2**:
  weights to optimize.
* **__group_86__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_86__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_86__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_86__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_87__weights** (optional) - **T2**:
  weights to optimize.
* **__group_87__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_87__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_87__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_87__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_88__weights** (optional) - **T2**:
  weights to optimize.
* **__group_88__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_88__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_88__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_88__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_89__weights** (optional) - **T2**:
  weights to optimize.
* **__group_89__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_89__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_89__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_89__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_90__weights** (optional) - **T2**:
  weights to optimize.
* **__group_90__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_90__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_90__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_90__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_91__weights** (optional) - **T2**:
  weights to optimize.
* **__group_91__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_91__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_91__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_91__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_92__weights** (optional) - **T2**:
  weights to optimize.
* **__group_92__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_92__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_92__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_92__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_93__weights** (optional) - **T2**:
  weights to optimize.
* **__group_93__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_93__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_93__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_93__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_94__weights** (optional) - **T2**:
  weights to optimize.
* **__group_94__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_94__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_94__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_94__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_95__weights** (optional) - **T2**:
  weights to optimize.
* **__group_95__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_95__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_95__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_95__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_96__weights** (optional) - **T2**:
  weights to optimize.
* **__group_96__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_96__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_96__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_96__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_97__weights** (optional) - **T2**:
  weights to optimize.
* **__group_97__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_97__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_97__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_97__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_98__weights** (optional) - **T2**:
  weights to optimize.
* **__group_98__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_98__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_98__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_98__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_99__weights** (optional) - **T2**:
  weights to optimize.
* **__group_99__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_99__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_99__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_99__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_100__weights** (optional) - **T2**:
  weights to optimize.
* **__group_100__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_100__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_100__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_100__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_101__weights** (optional) - **T2**:
  weights to optimize.
* **__group_101__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_101__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_101__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_101__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_102__weights** (optional) - **T2**:
  weights to optimize.
* **__group_102__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_102__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_102__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_102__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_103__weights** (optional) - **T2**:
  weights to optimize.
* **__group_103__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_103__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_103__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_103__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_104__weights** (optional) - **T2**:
  weights to optimize.
* **__group_104__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_104__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_104__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_104__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_105__weights** (optional) - **T2**:
  weights to optimize.
* **__group_105__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_105__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_105__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_105__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_106__weights** (optional) - **T2**:
  weights to optimize.
* **__group_106__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_106__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_106__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_106__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_107__weights** (optional) - **T2**:
  weights to optimize.
* **__group_107__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_107__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_107__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_107__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_108__weights** (optional) - **T2**:
  weights to optimize.
* **__group_108__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_108__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_108__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_108__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_109__weights** (optional) - **T2**:
  weights to optimize.
* **__group_109__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_109__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_109__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_109__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_110__weights** (optional) - **T2**:
  weights to optimize.
* **__group_110__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_110__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_110__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_110__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_111__weights** (optional) - **T2**:
  weights to optimize.
* **__group_111__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_111__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_111__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_111__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_112__weights** (optional) - **T2**:
  weights to optimize.
* **__group_112__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_112__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_112__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_112__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_113__weights** (optional) - **T2**:
  weights to optimize.
* **__group_113__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_113__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_113__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_113__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_114__weights** (optional) - **T2**:
  weights to optimize.
* **__group_114__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_114__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_114__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_114__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_115__weights** (optional) - **T2**:
  weights to optimize.
* **__group_115__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_115__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_115__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_115__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_116__weights** (optional) - **T2**:
  weights to optimize.
* **__group_116__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_116__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_116__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_116__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_117__weights** (optional) - **T2**:
  weights to optimize.
* **__group_117__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_117__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_117__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_117__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_118__weights** (optional) - **T2**:
  weights to optimize.
* **__group_118__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_118__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_118__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_118__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_119__weights** (optional) - **T2**:
  weights to optimize.
* **__group_119__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_119__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_119__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_119__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_120__weights** (optional) - **T2**:
  weights to optimize.
* **__group_120__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_120__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_120__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_120__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_121__weights** (optional) - **T2**:
  weights to optimize.
* **__group_121__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_121__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_121__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_121__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_122__weights** (optional) - **T2**:
  weights to optimize.
* **__group_122__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_122__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_122__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_122__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_123__weights** (optional) - **T2**:
  weights to optimize.
* **__group_123__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_123__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_123__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_123__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_124__weights** (optional) - **T2**:
  weights to optimize.
* **__group_124__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_124__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_124__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_124__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_125__weights** (optional) - **T2**:
  weights to optimize.
* **__group_125__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_125__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_125__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_125__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_126__weights** (optional) - **T2**:
  weights to optimize.
* **__group_126__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_126__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_126__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_126__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_127__weights** (optional) - **T2**:
  weights to optimize.
* **__group_127__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_127__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_127__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_127__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_128__weights** (optional) - **T2**:
  weights to optimize.
* **__group_128__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_128__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_128__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_128__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_129__weights** (optional) - **T2**:
  weights to optimize.
* **__group_129__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_129__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_129__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_129__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_130__weights** (optional) - **T2**:
  weights to optimize.
* **__group_130__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_130__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_130__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_130__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_131__weights** (optional) - **T2**:
  weights to optimize.
* **__group_131__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_131__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_131__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_131__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_132__weights** (optional) - **T2**:
  weights to optimize.
* **__group_132__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_132__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_132__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_132__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_133__weights** (optional) - **T2**:
  weights to optimize.
* **__group_133__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_133__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_133__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_133__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_134__weights** (optional) - **T2**:
  weights to optimize.
* **__group_134__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_134__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_134__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_134__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_135__weights** (optional) - **T2**:
  weights to optimize.
* **__group_135__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_135__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_135__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_135__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_136__weights** (optional) - **T2**:
  weights to optimize.
* **__group_136__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_136__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_136__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_136__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_137__weights** (optional) - **T2**:
  weights to optimize.
* **__group_137__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_137__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_137__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_137__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_138__weights** (optional) - **T2**:
  weights to optimize.
* **__group_138__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_138__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_138__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_138__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_139__weights** (optional) - **T2**:
  weights to optimize.
* **__group_139__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_139__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_139__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_139__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_140__weights** (optional) - **T2**:
  weights to optimize.
* **__group_140__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_140__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_140__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_140__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_141__weights** (optional) - **T2**:
  weights to optimize.
* **__group_141__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_141__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_141__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_141__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_142__weights** (optional) - **T2**:
  weights to optimize.
* **__group_142__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_142__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_142__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_142__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_143__weights** (optional) - **T2**:
  weights to optimize.
* **__group_143__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_143__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_143__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_143__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_144__weights** (optional) - **T2**:
  weights to optimize.
* **__group_144__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_144__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_144__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_144__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_145__weights** (optional) - **T2**:
  weights to optimize.
* **__group_145__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_145__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_145__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_145__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_146__weights** (optional) - **T2**:
  weights to optimize.
* **__group_146__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_146__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_146__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_146__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_147__weights** (optional) - **T2**:
  weights to optimize.
* **__group_147__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_147__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_147__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_147__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_148__weights** (optional) - **T2**:
  weights to optimize.
* **__group_148__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_148__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_148__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_148__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_149__weights** (optional) - **T2**:
  weights to optimize.
* **__group_149__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_149__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_149__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_149__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_150__weights** (optional) - **T2**:
  weights to optimize.
* **__group_150__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_150__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_150__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_150__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_151__weights** (optional) - **T2**:
  weights to optimize.
* **__group_151__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_151__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_151__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_151__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_152__weights** (optional) - **T2**:
  weights to optimize.
* **__group_152__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_152__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_152__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_152__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_153__weights** (optional) - **T2**:
  weights to optimize.
* **__group_153__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_153__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_153__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_153__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_154__weights** (optional) - **T2**:
  weights to optimize.
* **__group_154__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_154__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_154__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_154__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_155__weights** (optional) - **T2**:
  weights to optimize.
* **__group_155__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_155__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_155__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_155__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_156__weights** (optional) - **T2**:
  weights to optimize.
* **__group_156__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_156__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_156__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_156__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_157__weights** (optional) - **T2**:
  weights to optimize.
* **__group_157__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_157__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_157__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_157__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_158__weights** (optional) - **T2**:
  weights to optimize.
* **__group_158__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_158__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_158__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_158__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_159__weights** (optional) - **T2**:
  weights to optimize.
* **__group_159__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_159__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_159__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_159__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_160__weights** (optional) - **T2**:
  weights to optimize.
* **__group_160__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_160__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_160__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_160__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_161__weights** (optional) - **T2**:
  weights to optimize.
* **__group_161__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_161__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_161__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_161__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_162__weights** (optional) - **T2**:
  weights to optimize.
* **__group_162__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_162__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_162__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_162__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_163__weights** (optional) - **T2**:
  weights to optimize.
* **__group_163__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_163__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_163__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_163__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_164__weights** (optional) - **T2**:
  weights to optimize.
* **__group_164__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_164__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_164__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_164__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_165__weights** (optional) - **T2**:
  weights to optimize.
* **__group_165__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_165__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_165__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_165__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_166__weights** (optional) - **T2**:
  weights to optimize.
* **__group_166__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_166__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_166__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_166__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_167__weights** (optional) - **T2**:
  weights to optimize.
* **__group_167__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_167__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_167__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_167__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_168__weights** (optional) - **T2**:
  weights to optimize.
* **__group_168__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_168__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_168__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_168__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_169__weights** (optional) - **T2**:
  weights to optimize.
* **__group_169__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_169__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_169__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_169__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_170__weights** (optional) - **T2**:
  weights to optimize.
* **__group_170__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_170__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_170__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_170__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_171__weights** (optional) - **T2**:
  weights to optimize.
* **__group_171__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_171__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_171__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_171__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_172__weights** (optional) - **T2**:
  weights to optimize.
* **__group_172__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_172__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_172__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_172__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_173__weights** (optional) - **T2**:
  weights to optimize.
* **__group_173__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_173__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_173__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_173__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_174__weights** (optional) - **T2**:
  weights to optimize.
* **__group_174__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_174__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_174__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_174__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_175__weights** (optional) - **T2**:
  weights to optimize.
* **__group_175__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_175__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_175__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_175__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_176__weights** (optional) - **T2**:
  weights to optimize.
* **__group_176__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_176__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_176__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_176__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_177__weights** (optional) - **T2**:
  weights to optimize.
* **__group_177__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_177__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_177__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_177__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_178__weights** (optional) - **T2**:
  weights to optimize.
* **__group_178__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_178__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_178__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_178__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_179__weights** (optional) - **T2**:
  weights to optimize.
* **__group_179__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_179__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_179__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_179__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_180__weights** (optional) - **T2**:
  weights to optimize.
* **__group_180__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_180__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_180__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_180__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_181__weights** (optional) - **T2**:
  weights to optimize.
* **__group_181__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_181__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_181__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_181__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_182__weights** (optional) - **T2**:
  weights to optimize.
* **__group_182__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_182__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_182__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_182__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_183__weights** (optional) - **T2**:
  weights to optimize.
* **__group_183__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_183__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_183__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_183__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_184__weights** (optional) - **T2**:
  weights to optimize.
* **__group_184__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_184__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_184__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_184__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_185__weights** (optional) - **T2**:
  weights to optimize.
* **__group_185__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_185__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_185__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_185__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_186__weights** (optional) - **T2**:
  weights to optimize.
* **__group_186__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_186__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_186__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_186__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_187__weights** (optional) - **T2**:
  weights to optimize.
* **__group_187__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_187__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_187__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_187__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_188__weights** (optional) - **T2**:
  weights to optimize.
* **__group_188__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_188__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_188__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_188__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_189__weights** (optional) - **T2**:
  weights to optimize.
* **__group_189__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_189__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_189__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_189__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_190__weights** (optional) - **T2**:
  weights to optimize.
* **__group_190__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_190__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_190__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_190__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_191__weights** (optional) - **T2**:
  weights to optimize.
* **__group_191__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_191__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_191__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_191__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_192__weights** (optional) - **T2**:
  weights to optimize.
* **__group_192__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_192__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_192__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_192__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_193__weights** (optional) - **T2**:
  weights to optimize.
* **__group_193__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_193__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_193__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_193__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_194__weights** (optional) - **T2**:
  weights to optimize.
* **__group_194__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_194__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_194__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_194__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_195__weights** (optional) - **T2**:
  weights to optimize.
* **__group_195__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_195__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_195__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_195__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_196__weights** (optional) - **T2**:
  weights to optimize.
* **__group_196__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_196__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_196__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_196__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_197__weights** (optional) - **T2**:
  weights to optimize.
* **__group_197__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_197__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_197__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_197__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_198__weights** (optional) - **T2**:
  weights to optimize.
* **__group_198__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_198__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_198__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_198__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_199__weights** (optional) - **T2**:
  weights to optimize.
* **__group_199__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_199__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_199__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_199__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_200__weights** (optional) - **T2**:
  weights to optimize.
* **__group_200__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_200__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_200__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_200__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_201__weights** (optional) - **T2**:
  weights to optimize.
* **__group_201__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_201__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_201__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_201__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_202__weights** (optional) - **T2**:
  weights to optimize.
* **__group_202__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_202__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_202__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_202__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_203__weights** (optional) - **T2**:
  weights to optimize.
* **__group_203__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_203__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_203__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_203__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_204__weights** (optional) - **T2**:
  weights to optimize.
* **__group_204__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_204__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_204__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_204__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_205__weights** (optional) - **T2**:
  weights to optimize.
* **__group_205__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_205__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_205__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_205__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_206__weights** (optional) - **T2**:
  weights to optimize.
* **__group_206__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_206__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_206__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_206__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_207__weights** (optional) - **T2**:
  weights to optimize.
* **__group_207__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_207__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_207__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_207__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_208__weights** (optional) - **T2**:
  weights to optimize.
* **__group_208__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_208__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_208__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_208__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_209__weights** (optional) - **T2**:
  weights to optimize.
* **__group_209__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_209__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_209__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_209__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_210__weights** (optional) - **T2**:
  weights to optimize.
* **__group_210__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_210__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_210__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_210__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_211__weights** (optional) - **T2**:
  weights to optimize.
* **__group_211__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_211__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_211__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_211__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_212__weights** (optional) - **T2**:
  weights to optimize.
* **__group_212__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_212__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_212__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_212__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_213__weights** (optional) - **T2**:
  weights to optimize.
* **__group_213__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_213__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_213__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_213__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_214__weights** (optional) - **T2**:
  weights to optimize.
* **__group_214__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_214__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_214__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_214__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_215__weights** (optional) - **T2**:
  weights to optimize.
* **__group_215__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_215__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_215__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_215__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_216__weights** (optional) - **T2**:
  weights to optimize.
* **__group_216__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_216__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_216__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_216__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_217__weights** (optional) - **T2**:
  weights to optimize.
* **__group_217__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_217__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_217__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_217__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_218__weights** (optional) - **T2**:
  weights to optimize.
* **__group_218__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_218__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_218__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_218__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_219__weights** (optional) - **T2**:
  weights to optimize.
* **__group_219__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_219__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_219__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_219__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_220__weights** (optional) - **T2**:
  weights to optimize.
* **__group_220__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_220__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_220__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_220__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_221__weights** (optional) - **T2**:
  weights to optimize.
* **__group_221__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_221__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_221__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_221__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_222__weights** (optional) - **T2**:
  weights to optimize.
* **__group_222__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_222__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_222__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_222__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_223__weights** (optional) - **T2**:
  weights to optimize.
* **__group_223__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_223__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_223__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_223__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_224__weights** (optional) - **T2**:
  weights to optimize.
* **__group_224__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_224__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_224__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_224__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_225__weights** (optional) - **T2**:
  weights to optimize.
* **__group_225__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_225__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_225__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_225__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_226__weights** (optional) - **T2**:
  weights to optimize.
* **__group_226__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_226__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_226__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_226__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_227__weights** (optional) - **T2**:
  weights to optimize.
* **__group_227__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_227__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_227__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_227__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_228__weights** (optional) - **T2**:
  weights to optimize.
* **__group_228__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_228__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_228__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_228__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_229__weights** (optional) - **T2**:
  weights to optimize.
* **__group_229__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_229__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_229__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_229__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_230__weights** (optional) - **T2**:
  weights to optimize.
* **__group_230__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_230__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_230__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_230__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_231__weights** (optional) - **T2**:
  weights to optimize.
* **__group_231__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_231__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_231__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_231__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_232__weights** (optional) - **T2**:
  weights to optimize.
* **__group_232__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_232__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_232__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_232__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_233__weights** (optional) - **T2**:
  weights to optimize.
* **__group_233__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_233__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_233__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_233__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_234__weights** (optional) - **T2**:
  weights to optimize.
* **__group_234__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_234__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_234__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_234__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_235__weights** (optional) - **T2**:
  weights to optimize.
* **__group_235__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_235__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_235__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_235__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_236__weights** (optional) - **T2**:
  weights to optimize.
* **__group_236__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_236__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_236__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_236__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_237__weights** (optional) - **T2**:
  weights to optimize.
* **__group_237__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_237__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_237__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_237__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_238__weights** (optional) - **T2**:
  weights to optimize.
* **__group_238__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_238__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_238__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_238__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_239__weights** (optional) - **T2**:
  weights to optimize.
* **__group_239__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_239__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_239__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_239__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_240__weights** (optional) - **T2**:
  weights to optimize.
* **__group_240__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_240__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_240__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_240__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_241__weights** (optional) - **T2**:
  weights to optimize.
* **__group_241__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_241__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_241__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_241__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_242__weights** (optional) - **T2**:
  weights to optimize.
* **__group_242__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_242__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_242__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_242__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_243__weights** (optional) - **T2**:
  weights to optimize.
* **__group_243__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_243__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_243__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_243__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_244__weights** (optional) - **T2**:
  weights to optimize.
* **__group_244__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_244__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_244__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_244__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_245__weights** (optional) - **T2**:
  weights to optimize.
* **__group_245__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_245__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_245__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_245__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_246__weights** (optional) - **T2**:
  weights to optimize.
* **__group_246__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_246__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_246__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_246__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_247__weights** (optional) - **T2**:
  weights to optimize.
* **__group_247__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_247__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_247__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_247__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_248__weights** (optional) - **T2**:
  weights to optimize.
* **__group_248__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_248__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_248__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_248__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_249__weights** (optional) - **T2**:
  weights to optimize.
* **__group_249__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_249__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_249__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_249__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_250__weights** (optional) - **T2**:
  weights to optimize.
* **__group_250__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_250__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_250__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_250__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_251__weights** (optional) - **T2**:
  weights to optimize.
* **__group_251__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_251__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_251__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_251__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_252__weights** (optional) - **T2**:
  weights to optimize.
* **__group_252__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_252__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_252__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_252__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_253__weights** (optional) - **T2**:
  weights to optimize.
* **__group_253__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_253__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_253__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_253__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_254__weights** (optional) - **T2**:
  weights to optimize.
* **__group_254__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_254__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_254__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_254__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_255__weights** (optional) - **T2**:
  weights to optimize.
* **__group_255__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_255__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_255__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_255__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_256__weights** (optional) - **T2**:
  weights to optimize.
* **__group_256__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_256__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_256__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_256__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_257__weights** (optional) - **T2**:
  weights to optimize.
* **__group_257__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_257__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_257__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_257__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_258__weights** (optional) - **T2**:
  weights to optimize.
* **__group_258__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_258__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_258__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_258__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_259__weights** (optional) - **T2**:
  weights to optimize.
* **__group_259__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_259__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_259__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_259__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_260__weights** (optional) - **T2**:
  weights to optimize.
* **__group_260__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_260__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_260__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_260__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_261__weights** (optional) - **T2**:
  weights to optimize.
* **__group_261__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_261__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_261__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_261__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_262__weights** (optional) - **T2**:
  weights to optimize.
* **__group_262__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_262__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_262__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_262__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_263__weights** (optional) - **T2**:
  weights to optimize.
* **__group_263__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_263__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_263__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_263__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_264__weights** (optional) - **T2**:
  weights to optimize.
* **__group_264__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_264__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_264__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_264__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_265__weights** (optional) - **T2**:
  weights to optimize.
* **__group_265__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_265__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_265__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_265__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_266__weights** (optional) - **T2**:
  weights to optimize.
* **__group_266__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_266__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_266__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_266__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_267__weights** (optional) - **T2**:
  weights to optimize.
* **__group_267__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_267__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_267__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_267__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_268__weights** (optional) - **T2**:
  weights to optimize.
* **__group_268__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_268__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_268__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_268__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_269__weights** (optional) - **T2**:
  weights to optimize.
* **__group_269__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_269__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_269__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_269__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_270__weights** (optional) - **T2**:
  weights to optimize.
* **__group_270__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_270__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_270__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_270__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_271__weights** (optional) - **T2**:
  weights to optimize.
* **__group_271__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_271__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_271__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_271__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_272__weights** (optional) - **T2**:
  weights to optimize.
* **__group_272__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_272__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_272__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_272__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_273__weights** (optional) - **T2**:
  weights to optimize.
* **__group_273__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_273__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_273__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_273__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_274__weights** (optional) - **T2**:
  weights to optimize.
* **__group_274__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_274__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_274__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_274__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_275__weights** (optional) - **T2**:
  weights to optimize.
* **__group_275__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_275__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_275__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_275__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_276__weights** (optional) - **T2**:
  weights to optimize.
* **__group_276__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_276__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_276__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_276__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_277__weights** (optional) - **T2**:
  weights to optimize.
* **__group_277__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_277__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_277__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_277__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_278__weights** (optional) - **T2**:
  weights to optimize.
* **__group_278__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_278__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_278__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_278__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_279__weights** (optional) - **T2**:
  weights to optimize.
* **__group_279__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_279__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_279__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_279__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_280__weights** (optional) - **T2**:
  weights to optimize.
* **__group_280__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_280__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_280__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_280__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_281__weights** (optional) - **T2**:
  weights to optimize.
* **__group_281__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_281__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_281__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_281__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_282__weights** (optional) - **T2**:
  weights to optimize.
* **__group_282__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_282__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_282__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_282__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_283__weights** (optional) - **T2**:
  weights to optimize.
* **__group_283__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_283__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_283__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_283__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_284__weights** (optional) - **T2**:
  weights to optimize.
* **__group_284__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_284__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_284__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_284__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_285__weights** (optional) - **T2**:
  weights to optimize.
* **__group_285__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_285__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_285__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_285__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_286__weights** (optional) - **T2**:
  weights to optimize.
* **__group_286__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_286__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_286__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_286__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_287__weights** (optional) - **T2**:
  weights to optimize.
* **__group_287__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_287__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_287__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_287__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_288__weights** (optional) - **T2**:
  weights to optimize.
* **__group_288__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_288__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_288__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_288__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_289__weights** (optional) - **T2**:
  weights to optimize.
* **__group_289__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_289__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_289__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_289__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_290__weights** (optional) - **T2**:
  weights to optimize.
* **__group_290__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_290__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_290__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_290__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_291__weights** (optional) - **T2**:
  weights to optimize.
* **__group_291__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_291__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_291__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_291__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_292__weights** (optional) - **T2**:
  weights to optimize.
* **__group_292__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_292__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_292__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_292__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_293__weights** (optional) - **T2**:
  weights to optimize.
* **__group_293__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_293__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_293__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_293__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_294__weights** (optional) - **T2**:
  weights to optimize.
* **__group_294__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_294__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_294__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_294__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_295__weights** (optional) - **T2**:
  weights to optimize.
* **__group_295__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_295__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_295__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_295__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_296__weights** (optional) - **T2**:
  weights to optimize.
* **__group_296__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_296__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_296__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_296__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_297__weights** (optional) - **T2**:
  weights to optimize.
* **__group_297__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_297__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_297__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_297__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_298__weights** (optional) - **T2**:
  weights to optimize.
* **__group_298__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_298__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_298__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_298__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_299__weights** (optional) - **T2**:
  weights to optimize.
* **__group_299__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_299__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_299__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_299__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_300__weights** (optional) - **T2**:
  weights to optimize.
* **__group_300__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_300__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_300__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_300__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_301__weights** (optional) - **T2**:
  weights to optimize.
* **__group_301__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_301__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_301__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_301__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_302__weights** (optional) - **T2**:
  weights to optimize.
* **__group_302__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_302__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_302__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_302__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_303__weights** (optional) - **T2**:
  weights to optimize.
* **__group_303__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_303__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_303__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_303__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_304__weights** (optional) - **T2**:
  weights to optimize.
* **__group_304__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_304__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_304__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_304__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_305__weights** (optional) - **T2**:
  weights to optimize.
* **__group_305__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_305__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_305__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_305__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_306__weights** (optional) - **T2**:
  weights to optimize.
* **__group_306__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_306__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_306__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_306__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_307__weights** (optional) - **T2**:
  weights to optimize.
* **__group_307__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_307__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_307__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_307__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_308__weights** (optional) - **T2**:
  weights to optimize.
* **__group_308__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_308__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_308__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_308__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_309__weights** (optional) - **T2**:
  weights to optimize.
* **__group_309__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_309__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_309__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_309__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_310__weights** (optional) - **T2**:
  weights to optimize.
* **__group_310__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_310__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_310__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_310__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_311__weights** (optional) - **T2**:
  weights to optimize.
* **__group_311__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_311__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_311__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_311__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_312__weights** (optional) - **T2**:
  weights to optimize.
* **__group_312__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_312__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_312__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_312__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_313__weights** (optional) - **T2**:
  weights to optimize.
* **__group_313__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_313__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_313__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_313__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_314__weights** (optional) - **T2**:
  weights to optimize.
* **__group_314__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_314__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_314__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_314__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_315__weights** (optional) - **T2**:
  weights to optimize.
* **__group_315__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_315__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_315__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_315__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_316__weights** (optional) - **T2**:
  weights to optimize.
* **__group_316__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_316__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_316__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_316__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_317__weights** (optional) - **T2**:
  weights to optimize.
* **__group_317__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_317__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_317__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_317__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_318__weights** (optional) - **T2**:
  weights to optimize.
* **__group_318__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_318__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_318__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_318__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_319__weights** (optional) - **T2**:
  weights to optimize.
* **__group_319__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_319__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_319__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_319__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_320__weights** (optional) - **T2**:
  weights to optimize.
* **__group_320__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_320__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_320__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_320__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_321__weights** (optional) - **T2**:
  weights to optimize.
* **__group_321__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_321__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_321__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_321__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_322__weights** (optional) - **T2**:
  weights to optimize.
* **__group_322__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_322__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_322__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_322__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_323__weights** (optional) - **T2**:
  weights to optimize.
* **__group_323__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_323__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_323__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_323__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_324__weights** (optional) - **T2**:
  weights to optimize.
* **__group_324__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_324__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_324__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_324__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_325__weights** (optional) - **T2**:
  weights to optimize.
* **__group_325__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_325__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_325__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_325__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_326__weights** (optional) - **T2**:
  weights to optimize.
* **__group_326__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_326__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_326__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_326__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_327__weights** (optional) - **T2**:
  weights to optimize.
* **__group_327__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_327__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_327__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_327__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_328__weights** (optional) - **T2**:
  weights to optimize.
* **__group_328__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_328__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_328__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_328__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_329__weights** (optional) - **T2**:
  weights to optimize.
* **__group_329__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_329__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_329__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_329__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_330__weights** (optional) - **T2**:
  weights to optimize.
* **__group_330__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_330__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_330__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_330__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_331__weights** (optional) - **T2**:
  weights to optimize.
* **__group_331__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_331__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_331__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_331__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_332__weights** (optional) - **T2**:
  weights to optimize.
* **__group_332__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_332__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_332__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_332__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_333__weights** (optional) - **T2**:
  weights to optimize.
* **__group_333__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_333__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_333__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_333__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_334__weights** (optional) - **T2**:
  weights to optimize.
* **__group_334__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_334__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_334__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_334__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_335__weights** (optional) - **T2**:
  weights to optimize.
* **__group_335__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_335__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_335__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_335__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_336__weights** (optional) - **T2**:
  weights to optimize.
* **__group_336__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_336__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_336__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_336__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_337__weights** (optional) - **T2**:
  weights to optimize.
* **__group_337__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_337__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_337__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_337__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_338__weights** (optional) - **T2**:
  weights to optimize.
* **__group_338__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_338__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_338__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_338__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_339__weights** (optional) - **T2**:
  weights to optimize.
* **__group_339__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_339__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_339__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_339__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_340__weights** (optional) - **T2**:
  weights to optimize.
* **__group_340__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_340__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_340__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_340__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_341__weights** (optional) - **T2**:
  weights to optimize.
* **__group_341__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_341__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_341__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_341__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_342__weights** (optional) - **T2**:
  weights to optimize.
* **__group_342__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_342__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_342__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_342__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_343__weights** (optional) - **T2**:
  weights to optimize.
* **__group_343__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_343__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_343__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_343__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_344__weights** (optional) - **T2**:
  weights to optimize.
* **__group_344__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_344__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_344__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_344__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_345__weights** (optional) - **T2**:
  weights to optimize.
* **__group_345__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_345__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_345__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_345__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_346__weights** (optional) - **T2**:
  weights to optimize.
* **__group_346__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_346__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_346__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_346__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_347__weights** (optional) - **T2**:
  weights to optimize.
* **__group_347__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_347__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_347__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_347__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_348__weights** (optional) - **T2**:
  weights to optimize.
* **__group_348__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_348__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_348__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_348__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_349__weights** (optional) - **T2**:
  weights to optimize.
* **__group_349__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_349__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_349__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_349__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_350__weights** (optional) - **T2**:
  weights to optimize.
* **__group_350__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_350__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_350__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_350__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_351__weights** (optional) - **T2**:
  weights to optimize.
* **__group_351__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_351__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_351__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_351__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_352__weights** (optional) - **T2**:
  weights to optimize.
* **__group_352__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_352__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_352__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_352__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_353__weights** (optional) - **T2**:
  weights to optimize.
* **__group_353__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_353__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_353__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_353__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_354__weights** (optional) - **T2**:
  weights to optimize.
* **__group_354__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_354__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_354__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_354__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_355__weights** (optional) - **T2**:
  weights to optimize.
* **__group_355__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_355__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_355__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_355__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_356__weights** (optional) - **T2**:
  weights to optimize.
* **__group_356__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_356__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_356__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_356__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_357__weights** (optional) - **T2**:
  weights to optimize.
* **__group_357__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_357__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_357__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_357__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_358__weights** (optional) - **T2**:
  weights to optimize.
* **__group_358__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_358__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_358__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_358__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_359__weights** (optional) - **T2**:
  weights to optimize.
* **__group_359__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_359__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_359__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_359__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_360__weights** (optional) - **T2**:
  weights to optimize.
* **__group_360__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_360__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_360__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_360__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_361__weights** (optional) - **T2**:
  weights to optimize.
* **__group_361__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_361__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_361__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_361__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_362__weights** (optional) - **T2**:
  weights to optimize.
* **__group_362__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_362__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_362__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_362__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_363__weights** (optional) - **T2**:
  weights to optimize.
* **__group_363__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_363__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_363__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_363__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_364__weights** (optional) - **T2**:
  weights to optimize.
* **__group_364__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_364__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_364__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_364__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_365__weights** (optional) - **T2**:
  weights to optimize.
* **__group_365__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_365__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_365__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_365__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_366__weights** (optional) - **T2**:
  weights to optimize.
* **__group_366__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_366__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_366__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_366__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_367__weights** (optional) - **T2**:
  weights to optimize.
* **__group_367__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_367__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_367__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_367__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_368__weights** (optional) - **T2**:
  weights to optimize.
* **__group_368__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_368__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_368__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_368__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_369__weights** (optional) - **T2**:
  weights to optimize.
* **__group_369__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_369__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_369__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_369__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_370__weights** (optional) - **T2**:
  weights to optimize.
* **__group_370__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_370__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_370__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_370__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_371__weights** (optional) - **T2**:
  weights to optimize.
* **__group_371__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_371__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_371__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_371__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_372__weights** (optional) - **T2**:
  weights to optimize.
* **__group_372__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_372__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_372__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_372__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_373__weights** (optional) - **T2**:
  weights to optimize.
* **__group_373__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_373__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_373__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_373__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_374__weights** (optional) - **T2**:
  weights to optimize.
* **__group_374__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_374__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_374__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_374__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_375__weights** (optional) - **T2**:
  weights to optimize.
* **__group_375__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_375__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_375__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_375__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_376__weights** (optional) - **T2**:
  weights to optimize.
* **__group_376__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_376__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_376__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_376__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_377__weights** (optional) - **T2**:
  weights to optimize.
* **__group_377__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_377__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_377__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_377__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_378__weights** (optional) - **T2**:
  weights to optimize.
* **__group_378__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_378__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_378__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_378__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_379__weights** (optional) - **T2**:
  weights to optimize.
* **__group_379__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_379__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_379__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_379__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_380__weights** (optional) - **T2**:
  weights to optimize.
* **__group_380__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_380__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_380__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_380__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_381__weights** (optional) - **T2**:
  weights to optimize.
* **__group_381__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_381__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_381__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_381__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_382__weights** (optional) - **T2**:
  weights to optimize.
* **__group_382__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_382__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_382__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_382__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_383__weights** (optional) - **T2**:
  weights to optimize.
* **__group_383__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_383__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_383__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_383__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_384__weights** (optional) - **T2**:
  weights to optimize.
* **__group_384__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_384__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_384__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_384__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_385__weights** (optional) - **T2**:
  weights to optimize.
* **__group_385__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_385__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_385__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_385__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_386__weights** (optional) - **T2**:
  weights to optimize.
* **__group_386__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_386__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_386__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_386__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_387__weights** (optional) - **T2**:
  weights to optimize.
* **__group_387__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_387__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_387__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_387__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_388__weights** (optional) - **T2**:
  weights to optimize.
* **__group_388__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_388__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_388__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_388__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_389__weights** (optional) - **T2**:
  weights to optimize.
* **__group_389__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_389__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_389__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_389__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_390__weights** (optional) - **T2**:
  weights to optimize.
* **__group_390__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_390__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_390__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_390__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_391__weights** (optional) - **T2**:
  weights to optimize.
* **__group_391__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_391__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_391__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_391__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_392__weights** (optional) - **T2**:
  weights to optimize.
* **__group_392__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_392__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_392__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_392__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_393__weights** (optional) - **T2**:
  weights to optimize.
* **__group_393__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_393__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_393__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_393__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_394__weights** (optional) - **T2**:
  weights to optimize.
* **__group_394__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_394__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_394__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_394__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_395__weights** (optional) - **T2**:
  weights to optimize.
* **__group_395__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_395__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_395__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_395__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_396__weights** (optional) - **T2**:
  weights to optimize.
* **__group_396__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_396__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_396__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_396__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_397__weights** (optional) - **T2**:
  weights to optimize.
* **__group_397__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_397__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_397__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_397__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_398__weights** (optional) - **T2**:
  weights to optimize.
* **__group_398__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_398__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_398__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_398__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_399__weights** (optional) - **T2**:
  weights to optimize.
* **__group_399__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_399__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_399__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_399__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_400__weights** (optional) - **T2**:
  weights to optimize.
* **__group_400__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_400__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_400__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_400__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_401__weights** (optional) - **T2**:
  weights to optimize.
* **__group_401__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_401__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_401__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_401__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_402__weights** (optional) - **T2**:
  weights to optimize.
* **__group_402__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_402__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_402__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_402__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_403__weights** (optional) - **T2**:
  weights to optimize.
* **__group_403__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_403__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_403__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_403__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_404__weights** (optional) - **T2**:
  weights to optimize.
* **__group_404__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_404__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_404__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_404__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_405__weights** (optional) - **T2**:
  weights to optimize.
* **__group_405__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_405__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_405__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_405__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_406__weights** (optional) - **T2**:
  weights to optimize.
* **__group_406__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_406__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_406__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_406__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_407__weights** (optional) - **T2**:
  weights to optimize.
* **__group_407__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_407__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_407__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_407__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_408__weights** (optional) - **T2**:
  weights to optimize.
* **__group_408__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_408__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_408__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_408__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_409__weights** (optional) - **T2**:
  weights to optimize.
* **__group_409__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_409__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_409__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_409__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_410__weights** (optional) - **T2**:
  weights to optimize.
* **__group_410__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_410__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_410__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_410__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_411__weights** (optional) - **T2**:
  weights to optimize.
* **__group_411__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_411__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_411__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_411__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_412__weights** (optional) - **T2**:
  weights to optimize.
* **__group_412__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_412__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_412__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_412__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_413__weights** (optional) - **T2**:
  weights to optimize.
* **__group_413__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_413__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_413__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_413__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_414__weights** (optional) - **T2**:
  weights to optimize.
* **__group_414__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_414__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_414__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_414__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_415__weights** (optional) - **T2**:
  weights to optimize.
* **__group_415__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_415__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_415__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_415__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_416__weights** (optional) - **T2**:
  weights to optimize.
* **__group_416__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_416__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_416__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_416__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_417__weights** (optional) - **T2**:
  weights to optimize.
* **__group_417__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_417__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_417__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_417__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_418__weights** (optional) - **T2**:
  weights to optimize.
* **__group_418__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_418__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_418__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_418__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_419__weights** (optional) - **T2**:
  weights to optimize.
* **__group_419__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_419__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_419__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_419__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_420__weights** (optional) - **T2**:
  weights to optimize.
* **__group_420__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_420__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_420__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_420__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_421__weights** (optional) - **T2**:
  weights to optimize.
* **__group_421__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_421__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_421__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_421__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_422__weights** (optional) - **T2**:
  weights to optimize.
* **__group_422__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_422__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_422__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_422__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_423__weights** (optional) - **T2**:
  weights to optimize.
* **__group_423__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_423__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_423__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_423__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_424__weights** (optional) - **T2**:
  weights to optimize.
* **__group_424__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_424__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_424__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_424__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_425__weights** (optional) - **T2**:
  weights to optimize.
* **__group_425__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_425__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_425__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_425__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_426__weights** (optional) - **T2**:
  weights to optimize.
* **__group_426__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_426__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_426__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_426__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_427__weights** (optional) - **T2**:
  weights to optimize.
* **__group_427__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_427__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_427__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_427__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_428__weights** (optional) - **T2**:
  weights to optimize.
* **__group_428__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_428__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_428__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_428__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_429__weights** (optional) - **T2**:
  weights to optimize.
* **__group_429__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_429__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_429__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_429__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_430__weights** (optional) - **T2**:
  weights to optimize.
* **__group_430__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_430__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_430__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_430__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_431__weights** (optional) - **T2**:
  weights to optimize.
* **__group_431__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_431__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_431__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_431__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_432__weights** (optional) - **T2**:
  weights to optimize.
* **__group_432__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_432__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_432__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_432__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_433__weights** (optional) - **T2**:
  weights to optimize.
* **__group_433__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_433__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_433__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_433__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_434__weights** (optional) - **T2**:
  weights to optimize.
* **__group_434__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_434__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_434__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_434__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_435__weights** (optional) - **T2**:
  weights to optimize.
* **__group_435__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_435__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_435__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_435__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_436__weights** (optional) - **T2**:
  weights to optimize.
* **__group_436__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_436__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_436__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_436__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_437__weights** (optional) - **T2**:
  weights to optimize.
* **__group_437__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_437__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_437__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_437__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_438__weights** (optional) - **T2**:
  weights to optimize.
* **__group_438__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_438__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_438__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_438__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_439__weights** (optional) - **T2**:
  weights to optimize.
* **__group_439__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_439__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_439__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_439__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_440__weights** (optional) - **T2**:
  weights to optimize.
* **__group_440__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_440__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_440__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_440__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_441__weights** (optional) - **T2**:
  weights to optimize.
* **__group_441__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_441__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_441__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_441__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_442__weights** (optional) - **T2**:
  weights to optimize.
* **__group_442__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_442__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_442__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_442__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_443__weights** (optional) - **T2**:
  weights to optimize.
* **__group_443__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_443__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_443__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_443__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_444__weights** (optional) - **T2**:
  weights to optimize.
* **__group_444__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_444__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_444__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_444__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_445__weights** (optional) - **T2**:
  weights to optimize.
* **__group_445__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_445__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_445__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_445__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_446__weights** (optional) - **T2**:
  weights to optimize.
* **__group_446__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_446__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_446__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_446__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_447__weights** (optional) - **T2**:
  weights to optimize.
* **__group_447__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_447__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_447__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_447__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_448__weights** (optional) - **T2**:
  weights to optimize.
* **__group_448__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_448__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_448__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_448__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_449__weights** (optional) - **T2**:
  weights to optimize.
* **__group_449__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_449__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_449__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_449__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_450__weights** (optional) - **T2**:
  weights to optimize.
* **__group_450__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_450__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_450__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_450__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_451__weights** (optional) - **T2**:
  weights to optimize.
* **__group_451__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_451__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_451__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_451__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_452__weights** (optional) - **T2**:
  weights to optimize.
* **__group_452__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_452__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_452__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_452__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_453__weights** (optional) - **T2**:
  weights to optimize.
* **__group_453__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_453__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_453__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_453__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_454__weights** (optional) - **T2**:
  weights to optimize.
* **__group_454__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_454__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_454__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_454__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_455__weights** (optional) - **T2**:
  weights to optimize.
* **__group_455__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_455__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_455__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_455__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_456__weights** (optional) - **T2**:
  weights to optimize.
* **__group_456__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_456__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_456__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_456__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_457__weights** (optional) - **T2**:
  weights to optimize.
* **__group_457__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_457__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_457__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_457__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_458__weights** (optional) - **T2**:
  weights to optimize.
* **__group_458__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_458__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_458__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_458__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_459__weights** (optional) - **T2**:
  weights to optimize.
* **__group_459__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_459__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_459__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_459__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_460__weights** (optional) - **T2**:
  weights to optimize.
* **__group_460__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_460__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_460__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_460__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_461__weights** (optional) - **T2**:
  weights to optimize.
* **__group_461__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_461__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_461__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_461__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_462__weights** (optional) - **T2**:
  weights to optimize.
* **__group_462__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_462__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_462__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_462__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_463__weights** (optional) - **T2**:
  weights to optimize.
* **__group_463__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_463__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_463__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_463__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_464__weights** (optional) - **T2**:
  weights to optimize.
* **__group_464__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_464__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_464__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_464__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_465__weights** (optional) - **T2**:
  weights to optimize.
* **__group_465__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_465__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_465__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_465__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_466__weights** (optional) - **T2**:
  weights to optimize.
* **__group_466__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_466__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_466__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_466__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_467__weights** (optional) - **T2**:
  weights to optimize.
* **__group_467__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_467__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_467__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_467__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_468__weights** (optional) - **T2**:
  weights to optimize.
* **__group_468__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_468__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_468__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_468__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_469__weights** (optional) - **T2**:
  weights to optimize.
* **__group_469__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_469__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_469__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_469__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_470__weights** (optional) - **T2**:
  weights to optimize.
* **__group_470__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_470__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_470__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_470__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_471__weights** (optional) - **T2**:
  weights to optimize.
* **__group_471__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_471__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_471__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_471__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_472__weights** (optional) - **T2**:
  weights to optimize.
* **__group_472__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_472__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_472__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_472__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_473__weights** (optional) - **T2**:
  weights to optimize.
* **__group_473__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_473__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_473__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_473__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_474__weights** (optional) - **T2**:
  weights to optimize.
* **__group_474__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_474__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_474__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_474__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_475__weights** (optional) - **T2**:
  weights to optimize.
* **__group_475__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_475__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_475__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_475__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_476__weights** (optional) - **T2**:
  weights to optimize.
* **__group_476__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_476__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_476__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_476__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_477__weights** (optional) - **T2**:
  weights to optimize.
* **__group_477__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_477__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_477__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_477__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_478__weights** (optional) - **T2**:
  weights to optimize.
* **__group_478__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_478__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_478__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_478__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_479__weights** (optional) - **T2**:
  weights to optimize.
* **__group_479__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_479__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_479__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_479__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_480__weights** (optional) - **T2**:
  weights to optimize.
* **__group_480__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_480__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_480__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_480__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_481__weights** (optional) - **T2**:
  weights to optimize.
* **__group_481__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_481__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_481__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_481__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_482__weights** (optional) - **T2**:
  weights to optimize.
* **__group_482__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_482__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_482__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_482__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_483__weights** (optional) - **T2**:
  weights to optimize.
* **__group_483__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_483__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_483__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_483__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_484__weights** (optional) - **T2**:
  weights to optimize.
* **__group_484__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_484__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_484__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_484__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_485__weights** (optional) - **T2**:
  weights to optimize.
* **__group_485__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_485__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_485__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_485__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_486__weights** (optional) - **T2**:
  weights to optimize.
* **__group_486__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_486__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_486__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_486__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_487__weights** (optional) - **T2**:
  weights to optimize.
* **__group_487__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_487__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_487__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_487__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_488__weights** (optional) - **T2**:
  weights to optimize.
* **__group_488__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_488__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_488__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_488__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_489__weights** (optional) - **T2**:
  weights to optimize.
* **__group_489__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_489__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_489__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_489__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_490__weights** (optional) - **T2**:
  weights to optimize.
* **__group_490__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_490__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_490__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_490__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_491__weights** (optional) - **T2**:
  weights to optimize.
* **__group_491__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_491__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_491__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_491__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_492__weights** (optional) - **T2**:
  weights to optimize.
* **__group_492__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_492__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_492__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_492__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_493__weights** (optional) - **T2**:
  weights to optimize.
* **__group_493__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_493__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_493__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_493__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_494__weights** (optional) - **T2**:
  weights to optimize.
* **__group_494__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_494__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_494__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_494__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_495__weights** (optional) - **T2**:
  weights to optimize.
* **__group_495__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_495__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_495__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_495__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_496__weights** (optional) - **T2**:
  weights to optimize.
* **__group_496__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_496__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_496__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_496__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_497__weights** (optional) - **T2**:
  weights to optimize.
* **__group_497__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_497__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_497__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_497__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_498__weights** (optional) - **T2**:
  weights to optimize.
* **__group_498__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_498__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_498__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_498__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_499__weights** (optional) - **T2**:
  weights to optimize.
* **__group_499__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_499__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_499__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_499__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_500__weights** (optional) - **T2**:
  weights to optimize.
* **__group_500__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_500__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_500__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_500__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_501__weights** (optional) - **T2**:
  weights to optimize.
* **__group_501__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_501__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_501__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_501__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_502__weights** (optional) - **T2**:
  weights to optimize.
* **__group_502__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_502__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_502__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_502__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_503__weights** (optional) - **T2**:
  weights to optimize.
* **__group_503__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_503__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_503__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_503__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_504__weights** (optional) - **T2**:
  weights to optimize.
* **__group_504__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_504__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_504__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_504__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_505__weights** (optional) - **T2**:
  weights to optimize.
* **__group_505__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_505__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_505__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_505__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_506__weights** (optional) - **T2**:
  weights to optimize.
* **__group_506__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_506__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_506__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_506__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_507__weights** (optional) - **T2**:
  weights to optimize.
* **__group_507__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_507__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_507__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_507__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_508__weights** (optional) - **T2**:
  weights to optimize.
* **__group_508__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_508__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_508__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_508__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_509__weights** (optional) - **T2**:
  weights to optimize.
* **__group_509__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_509__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_509__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_509__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_510__weights** (optional) - **T2**:
  weights to optimize.
* **__group_510__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_510__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_510__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_510__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_511__weights** (optional) - **T2**:
  weights to optimize.
* **__group_511__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_511__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_511__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_511__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_512__weights** (optional) - **T2**:
  weights to optimize.
* **__group_512__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_512__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_512__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_512__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_513__weights** (optional) - **T2**:
  weights to optimize.
* **__group_513__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_513__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_513__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_513__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_514__weights** (optional) - **T2**:
  weights to optimize.
* **__group_514__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_514__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_514__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_514__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_515__weights** (optional) - **T2**:
  weights to optimize.
* **__group_515__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_515__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_515__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_515__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_516__weights** (optional) - **T2**:
  weights to optimize.
* **__group_516__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_516__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_516__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_516__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_517__weights** (optional) - **T2**:
  weights to optimize.
* **__group_517__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_517__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_517__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_517__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_518__weights** (optional) - **T2**:
  weights to optimize.
* **__group_518__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_518__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_518__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_518__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_519__weights** (optional) - **T2**:
  weights to optimize.
* **__group_519__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_519__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_519__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_519__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_520__weights** (optional) - **T2**:
  weights to optimize.
* **__group_520__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_520__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_520__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_520__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_521__weights** (optional) - **T2**:
  weights to optimize.
* **__group_521__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_521__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_521__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_521__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_522__weights** (optional) - **T2**:
  weights to optimize.
* **__group_522__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_522__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_522__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_522__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_523__weights** (optional) - **T2**:
  weights to optimize.
* **__group_523__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_523__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_523__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_523__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_524__weights** (optional) - **T2**:
  weights to optimize.
* **__group_524__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_524__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_524__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_524__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_525__weights** (optional) - **T2**:
  weights to optimize.
* **__group_525__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_525__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_525__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_525__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_526__weights** (optional) - **T2**:
  weights to optimize.
* **__group_526__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_526__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_526__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_526__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_527__weights** (optional) - **T2**:
  weights to optimize.
* **__group_527__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_527__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_527__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_527__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_528__weights** (optional) - **T2**:
  weights to optimize.
* **__group_528__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_528__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_528__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_528__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_529__weights** (optional) - **T2**:
  weights to optimize.
* **__group_529__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_529__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_529__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_529__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_530__weights** (optional) - **T2**:
  weights to optimize.
* **__group_530__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_530__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_530__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_530__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_531__weights** (optional) - **T2**:
  weights to optimize.
* **__group_531__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_531__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_531__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_531__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_532__weights** (optional) - **T2**:
  weights to optimize.
* **__group_532__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_532__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_532__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_532__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_533__weights** (optional) - **T2**:
  weights to optimize.
* **__group_533__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_533__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_533__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_533__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_534__weights** (optional) - **T2**:
  weights to optimize.
* **__group_534__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_534__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_534__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_534__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_535__weights** (optional) - **T2**:
  weights to optimize.
* **__group_535__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_535__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_535__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_535__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_536__weights** (optional) - **T2**:
  weights to optimize.
* **__group_536__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_536__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_536__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_536__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_537__weights** (optional) - **T2**:
  weights to optimize.
* **__group_537__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_537__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_537__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_537__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_538__weights** (optional) - **T2**:
  weights to optimize.
* **__group_538__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_538__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_538__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_538__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_539__weights** (optional) - **T2**:
  weights to optimize.
* **__group_539__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_539__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_539__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_539__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_540__weights** (optional) - **T2**:
  weights to optimize.
* **__group_540__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_540__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_540__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_540__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_541__weights** (optional) - **T2**:
  weights to optimize.
* **__group_541__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_541__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_541__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_541__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_542__weights** (optional) - **T2**:
  weights to optimize.
* **__group_542__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_542__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_542__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_542__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_543__weights** (optional) - **T2**:
  weights to optimize.
* **__group_543__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_543__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_543__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_543__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_544__weights** (optional) - **T2**:
  weights to optimize.
* **__group_544__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_544__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_544__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_544__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_545__weights** (optional) - **T2**:
  weights to optimize.
* **__group_545__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_545__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_545__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_545__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_546__weights** (optional) - **T2**:
  weights to optimize.
* **__group_546__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_546__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_546__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_546__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_547__weights** (optional) - **T2**:
  weights to optimize.
* **__group_547__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_547__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_547__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_547__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_548__weights** (optional) - **T2**:
  weights to optimize.
* **__group_548__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_548__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_548__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_548__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_549__weights** (optional) - **T2**:
  weights to optimize.
* **__group_549__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_549__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_549__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_549__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_550__weights** (optional) - **T2**:
  weights to optimize.
* **__group_550__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_550__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_550__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_550__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_551__weights** (optional) - **T2**:
  weights to optimize.
* **__group_551__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_551__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_551__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_551__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_552__weights** (optional) - **T2**:
  weights to optimize.
* **__group_552__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_552__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_552__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_552__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_553__weights** (optional) - **T2**:
  weights to optimize.
* **__group_553__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_553__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_553__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_553__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_554__weights** (optional) - **T2**:
  weights to optimize.
* **__group_554__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_554__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_554__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_554__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_555__weights** (optional) - **T2**:
  weights to optimize.
* **__group_555__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_555__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_555__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_555__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_556__weights** (optional) - **T2**:
  weights to optimize.
* **__group_556__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_556__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_556__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_556__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_557__weights** (optional) - **T2**:
  weights to optimize.
* **__group_557__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_557__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_557__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_557__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_558__weights** (optional) - **T2**:
  weights to optimize.
* **__group_558__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_558__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_558__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_558__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_559__weights** (optional) - **T2**:
  weights to optimize.
* **__group_559__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_559__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_559__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_559__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_560__weights** (optional) - **T2**:
  weights to optimize.
* **__group_560__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_560__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_560__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_560__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_561__weights** (optional) - **T2**:
  weights to optimize.
* **__group_561__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_561__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_561__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_561__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_562__weights** (optional) - **T2**:
  weights to optimize.
* **__group_562__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_562__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_562__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_562__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_563__weights** (optional) - **T2**:
  weights to optimize.
* **__group_563__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_563__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_563__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_563__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_564__weights** (optional) - **T2**:
  weights to optimize.
* **__group_564__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_564__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_564__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_564__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_565__weights** (optional) - **T2**:
  weights to optimize.
* **__group_565__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_565__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_565__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_565__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_566__weights** (optional) - **T2**:
  weights to optimize.
* **__group_566__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_566__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_566__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_566__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_567__weights** (optional) - **T2**:
  weights to optimize.
* **__group_567__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_567__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_567__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_567__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_568__weights** (optional) - **T2**:
  weights to optimize.
* **__group_568__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_568__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_568__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_568__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_569__weights** (optional) - **T2**:
  weights to optimize.
* **__group_569__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_569__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_569__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_569__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_570__weights** (optional) - **T2**:
  weights to optimize.
* **__group_570__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_570__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_570__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_570__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_571__weights** (optional) - **T2**:
  weights to optimize.
* **__group_571__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_571__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_571__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_571__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_572__weights** (optional) - **T2**:
  weights to optimize.
* **__group_572__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_572__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_572__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_572__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_573__weights** (optional) - **T2**:
  weights to optimize.
* **__group_573__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_573__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_573__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_573__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_574__weights** (optional) - **T2**:
  weights to optimize.
* **__group_574__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_574__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_574__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_574__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_575__weights** (optional) - **T2**:
  weights to optimize.
* **__group_575__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_575__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_575__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_575__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_576__weights** (optional) - **T2**:
  weights to optimize.
* **__group_576__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_576__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_576__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_576__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_577__weights** (optional) - **T2**:
  weights to optimize.
* **__group_577__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_577__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_577__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_577__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_578__weights** (optional) - **T2**:
  weights to optimize.
* **__group_578__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_578__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_578__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_578__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_579__weights** (optional) - **T2**:
  weights to optimize.
* **__group_579__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_579__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_579__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_579__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_580__weights** (optional) - **T2**:
  weights to optimize.
* **__group_580__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_580__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_580__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_580__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_581__weights** (optional) - **T2**:
  weights to optimize.
* **__group_581__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_581__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_581__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_581__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_582__weights** (optional) - **T2**:
  weights to optimize.
* **__group_582__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_582__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_582__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_582__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_583__weights** (optional) - **T2**:
  weights to optimize.
* **__group_583__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_583__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_583__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_583__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_584__weights** (optional) - **T2**:
  weights to optimize.
* **__group_584__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_584__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_584__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_584__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_585__weights** (optional) - **T2**:
  weights to optimize.
* **__group_585__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_585__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_585__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_585__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_586__weights** (optional) - **T2**:
  weights to optimize.
* **__group_586__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_586__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_586__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_586__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_587__weights** (optional) - **T2**:
  weights to optimize.
* **__group_587__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_587__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_587__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_587__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_588__weights** (optional) - **T2**:
  weights to optimize.
* **__group_588__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_588__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_588__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_588__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_589__weights** (optional) - **T2**:
  weights to optimize.
* **__group_589__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_589__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_589__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_589__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_590__weights** (optional) - **T2**:
  weights to optimize.
* **__group_590__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_590__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_590__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_590__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_591__weights** (optional) - **T2**:
  weights to optimize.
* **__group_591__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_591__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_591__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_591__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_592__weights** (optional) - **T2**:
  weights to optimize.
* **__group_592__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_592__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_592__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_592__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_593__weights** (optional) - **T2**:
  weights to optimize.
* **__group_593__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_593__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_593__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_593__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_594__weights** (optional) - **T2**:
  weights to optimize.
* **__group_594__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_594__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_594__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_594__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_595__weights** (optional) - **T2**:
  weights to optimize.
* **__group_595__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_595__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_595__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_595__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_596__weights** (optional) - **T2**:
  weights to optimize.
* **__group_596__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_596__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_596__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_596__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_597__weights** (optional) - **T2**:
  weights to optimize.
* **__group_597__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_597__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_597__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_597__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_598__weights** (optional) - **T2**:
  weights to optimize.
* **__group_598__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_598__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_598__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_598__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_599__weights** (optional) - **T2**:
  weights to optimize.
* **__group_599__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_599__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_599__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_599__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_600__weights** (optional) - **T2**:
  weights to optimize.
* **__group_600__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_600__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_600__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_600__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_601__weights** (optional) - **T2**:
  weights to optimize.
* **__group_601__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_601__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_601__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_601__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_602__weights** (optional) - **T2**:
  weights to optimize.
* **__group_602__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_602__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_602__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_602__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_603__weights** (optional) - **T2**:
  weights to optimize.
* **__group_603__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_603__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_603__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_603__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_604__weights** (optional) - **T2**:
  weights to optimize.
* **__group_604__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_604__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_604__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_604__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_605__weights** (optional) - **T2**:
  weights to optimize.
* **__group_605__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_605__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_605__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_605__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_606__weights** (optional) - **T2**:
  weights to optimize.
* **__group_606__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_606__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_606__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_606__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_607__weights** (optional) - **T2**:
  weights to optimize.
* **__group_607__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_607__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_607__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_607__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_608__weights** (optional) - **T2**:
  weights to optimize.
* **__group_608__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_608__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_608__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_608__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_609__weights** (optional) - **T2**:
  weights to optimize.
* **__group_609__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_609__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_609__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_609__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_610__weights** (optional) - **T2**:
  weights to optimize.
* **__group_610__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_610__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_610__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_610__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_611__weights** (optional) - **T2**:
  weights to optimize.
* **__group_611__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_611__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_611__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_611__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_612__weights** (optional) - **T2**:
  weights to optimize.
* **__group_612__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_612__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_612__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_612__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_613__weights** (optional) - **T2**:
  weights to optimize.
* **__group_613__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_613__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_613__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_613__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_614__weights** (optional) - **T2**:
  weights to optimize.
* **__group_614__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_614__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_614__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_614__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_615__weights** (optional) - **T2**:
  weights to optimize.
* **__group_615__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_615__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_615__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_615__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_616__weights** (optional) - **T2**:
  weights to optimize.
* **__group_616__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_616__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_616__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_616__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_617__weights** (optional) - **T2**:
  weights to optimize.
* **__group_617__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_617__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_617__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_617__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_618__weights** (optional) - **T2**:
  weights to optimize.
* **__group_618__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_618__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_618__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_618__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_619__weights** (optional) - **T2**:
  weights to optimize.
* **__group_619__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_619__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_619__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_619__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_620__weights** (optional) - **T2**:
  weights to optimize.
* **__group_620__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_620__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_620__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_620__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_621__weights** (optional) - **T2**:
  weights to optimize.
* **__group_621__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_621__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_621__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_621__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_622__weights** (optional) - **T2**:
  weights to optimize.
* **__group_622__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_622__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_622__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_622__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_623__weights** (optional) - **T2**:
  weights to optimize.
* **__group_623__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_623__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_623__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_623__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_624__weights** (optional) - **T2**:
  weights to optimize.
* **__group_624__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_624__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_624__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_624__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_625__weights** (optional) - **T2**:
  weights to optimize.
* **__group_625__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_625__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_625__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_625__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_626__weights** (optional) - **T2**:
  weights to optimize.
* **__group_626__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_626__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_626__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_626__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_627__weights** (optional) - **T2**:
  weights to optimize.
* **__group_627__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_627__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_627__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_627__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_628__weights** (optional) - **T2**:
  weights to optimize.
* **__group_628__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_628__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_628__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_628__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_629__weights** (optional) - **T2**:
  weights to optimize.
* **__group_629__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_629__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_629__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_629__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_630__weights** (optional) - **T2**:
  weights to optimize.
* **__group_630__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_630__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_630__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_630__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_631__weights** (optional) - **T2**:
  weights to optimize.
* **__group_631__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_631__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_631__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_631__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_632__weights** (optional) - **T2**:
  weights to optimize.
* **__group_632__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_632__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_632__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_632__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_633__weights** (optional) - **T2**:
  weights to optimize.
* **__group_633__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_633__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_633__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_633__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_634__weights** (optional) - **T2**:
  weights to optimize.
* **__group_634__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_634__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_634__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_634__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_635__weights** (optional) - **T2**:
  weights to optimize.
* **__group_635__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_635__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_635__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_635__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_636__weights** (optional) - **T2**:
  weights to optimize.
* **__group_636__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_636__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_636__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_636__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_637__weights** (optional) - **T2**:
  weights to optimize.
* **__group_637__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_637__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_637__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_637__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_638__weights** (optional) - **T2**:
  weights to optimize.
* **__group_638__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_638__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_638__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_638__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_639__weights** (optional) - **T2**:
  weights to optimize.
* **__group_639__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_639__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_639__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_639__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_640__weights** (optional) - **T2**:
  weights to optimize.
* **__group_640__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_640__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_640__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_640__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_641__weights** (optional) - **T2**:
  weights to optimize.
* **__group_641__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_641__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_641__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_641__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_642__weights** (optional) - **T2**:
  weights to optimize.
* **__group_642__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_642__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_642__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_642__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_643__weights** (optional) - **T2**:
  weights to optimize.
* **__group_643__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_643__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_643__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_643__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_644__weights** (optional) - **T2**:
  weights to optimize.
* **__group_644__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_644__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_644__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_644__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_645__weights** (optional) - **T2**:
  weights to optimize.
* **__group_645__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_645__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_645__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_645__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_646__weights** (optional) - **T2**:
  weights to optimize.
* **__group_646__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_646__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_646__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_646__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_647__weights** (optional) - **T2**:
  weights to optimize.
* **__group_647__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_647__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_647__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_647__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_648__weights** (optional) - **T2**:
  weights to optimize.
* **__group_648__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_648__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_648__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_648__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_649__weights** (optional) - **T2**:
  weights to optimize.
* **__group_649__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_649__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_649__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_649__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_650__weights** (optional) - **T2**:
  weights to optimize.
* **__group_650__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_650__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_650__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_650__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_651__weights** (optional) - **T2**:
  weights to optimize.
* **__group_651__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_651__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_651__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_651__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_652__weights** (optional) - **T2**:
  weights to optimize.
* **__group_652__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_652__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_652__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_652__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_653__weights** (optional) - **T2**:
  weights to optimize.
* **__group_653__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_653__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_653__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_653__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_654__weights** (optional) - **T2**:
  weights to optimize.
* **__group_654__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_654__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_654__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_654__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_655__weights** (optional) - **T2**:
  weights to optimize.
* **__group_655__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_655__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_655__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_655__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_656__weights** (optional) - **T2**:
  weights to optimize.
* **__group_656__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_656__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_656__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_656__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_657__weights** (optional) - **T2**:
  weights to optimize.
* **__group_657__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_657__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_657__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_657__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_658__weights** (optional) - **T2**:
  weights to optimize.
* **__group_658__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_658__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_658__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_658__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_659__weights** (optional) - **T2**:
  weights to optimize.
* **__group_659__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_659__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_659__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_659__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_660__weights** (optional) - **T2**:
  weights to optimize.
* **__group_660__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_660__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_660__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_660__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_661__weights** (optional) - **T2**:
  weights to optimize.
* **__group_661__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_661__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_661__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_661__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_662__weights** (optional) - **T2**:
  weights to optimize.
* **__group_662__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_662__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_662__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_662__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_663__weights** (optional) - **T2**:
  weights to optimize.
* **__group_663__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_663__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_663__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_663__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_664__weights** (optional) - **T2**:
  weights to optimize.
* **__group_664__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_664__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_664__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_664__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_665__weights** (optional) - **T2**:
  weights to optimize.
* **__group_665__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_665__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_665__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_665__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_666__weights** (optional) - **T2**:
  weights to optimize.
* **__group_666__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_666__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_666__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_666__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_667__weights** (optional) - **T2**:
  weights to optimize.
* **__group_667__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_667__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_667__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_667__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_668__weights** (optional) - **T2**:
  weights to optimize.
* **__group_668__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_668__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_668__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_668__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_669__weights** (optional) - **T2**:
  weights to optimize.
* **__group_669__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_669__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_669__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_669__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_670__weights** (optional) - **T2**:
  weights to optimize.
* **__group_670__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_670__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_670__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_670__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_671__weights** (optional) - **T2**:
  weights to optimize.
* **__group_671__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_671__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_671__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_671__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_672__weights** (optional) - **T2**:
  weights to optimize.
* **__group_672__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_672__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_672__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_672__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_673__weights** (optional) - **T2**:
  weights to optimize.
* **__group_673__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_673__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_673__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_673__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_674__weights** (optional) - **T2**:
  weights to optimize.
* **__group_674__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_674__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_674__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_674__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_675__weights** (optional) - **T2**:
  weights to optimize.
* **__group_675__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_675__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_675__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_675__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_676__weights** (optional) - **T2**:
  weights to optimize.
* **__group_676__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_676__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_676__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_676__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_677__weights** (optional) - **T2**:
  weights to optimize.
* **__group_677__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_677__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_677__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_677__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_678__weights** (optional) - **T2**:
  weights to optimize.
* **__group_678__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_678__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_678__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_678__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_679__weights** (optional) - **T2**:
  weights to optimize.
* **__group_679__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_679__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_679__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_679__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_680__weights** (optional) - **T2**:
  weights to optimize.
* **__group_680__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_680__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_680__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_680__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_681__weights** (optional) - **T2**:
  weights to optimize.
* **__group_681__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_681__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_681__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_681__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_682__weights** (optional) - **T2**:
  weights to optimize.
* **__group_682__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_682__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_682__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_682__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_683__weights** (optional) - **T2**:
  weights to optimize.
* **__group_683__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_683__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_683__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_683__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_684__weights** (optional) - **T2**:
  weights to optimize.
* **__group_684__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_684__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_684__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_684__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_685__weights** (optional) - **T2**:
  weights to optimize.
* **__group_685__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_685__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_685__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_685__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_686__weights** (optional) - **T2**:
  weights to optimize.
* **__group_686__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_686__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_686__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_686__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_687__weights** (optional) - **T2**:
  weights to optimize.
* **__group_687__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_687__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_687__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_687__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_688__weights** (optional) - **T2**:
  weights to optimize.
* **__group_688__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_688__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_688__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_688__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_689__weights** (optional) - **T2**:
  weights to optimize.
* **__group_689__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_689__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_689__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_689__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_690__weights** (optional) - **T2**:
  weights to optimize.
* **__group_690__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_690__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_690__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_690__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_691__weights** (optional) - **T2**:
  weights to optimize.
* **__group_691__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_691__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_691__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_691__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_692__weights** (optional) - **T2**:
  weights to optimize.
* **__group_692__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_692__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_692__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_692__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_693__weights** (optional) - **T2**:
  weights to optimize.
* **__group_693__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_693__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_693__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_693__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_694__weights** (optional) - **T2**:
  weights to optimize.
* **__group_694__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_694__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_694__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_694__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_695__weights** (optional) - **T2**:
  weights to optimize.
* **__group_695__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_695__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_695__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_695__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_696__weights** (optional) - **T2**:
  weights to optimize.
* **__group_696__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_696__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_696__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_696__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_697__weights** (optional) - **T2**:
  weights to optimize.
* **__group_697__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_697__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_697__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_697__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_698__weights** (optional) - **T2**:
  weights to optimize.
* **__group_698__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_698__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_698__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_698__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_699__weights** (optional) - **T2**:
  weights to optimize.
* **__group_699__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_699__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_699__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_699__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_700__weights** (optional) - **T2**:
  weights to optimize.
* **__group_700__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_700__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_700__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_700__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_701__weights** (optional) - **T2**:
  weights to optimize.
* **__group_701__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_701__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_701__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_701__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_702__weights** (optional) - **T2**:
  weights to optimize.
* **__group_702__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_702__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_702__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_702__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_703__weights** (optional) - **T2**:
  weights to optimize.
* **__group_703__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_703__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_703__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_703__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_704__weights** (optional) - **T2**:
  weights to optimize.
* **__group_704__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_704__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_704__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_704__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_705__weights** (optional) - **T2**:
  weights to optimize.
* **__group_705__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_705__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_705__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_705__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_706__weights** (optional) - **T2**:
  weights to optimize.
* **__group_706__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_706__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_706__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_706__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_707__weights** (optional) - **T2**:
  weights to optimize.
* **__group_707__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_707__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_707__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_707__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_708__weights** (optional) - **T2**:
  weights to optimize.
* **__group_708__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_708__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_708__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_708__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_709__weights** (optional) - **T2**:
  weights to optimize.
* **__group_709__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_709__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_709__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_709__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_710__weights** (optional) - **T2**:
  weights to optimize.
* **__group_710__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_710__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_710__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_710__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_711__weights** (optional) - **T2**:
  weights to optimize.
* **__group_711__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_711__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_711__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_711__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_712__weights** (optional) - **T2**:
  weights to optimize.
* **__group_712__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_712__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_712__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_712__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_713__weights** (optional) - **T2**:
  weights to optimize.
* **__group_713__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_713__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_713__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_713__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_714__weights** (optional) - **T2**:
  weights to optimize.
* **__group_714__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_714__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_714__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_714__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_715__weights** (optional) - **T2**:
  weights to optimize.
* **__group_715__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_715__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_715__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_715__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_716__weights** (optional) - **T2**:
  weights to optimize.
* **__group_716__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_716__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_716__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_716__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_717__weights** (optional) - **T2**:
  weights to optimize.
* **__group_717__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_717__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_717__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_717__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_718__weights** (optional) - **T2**:
  weights to optimize.
* **__group_718__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_718__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_718__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_718__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_719__weights** (optional) - **T2**:
  weights to optimize.
* **__group_719__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_719__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_719__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_719__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_720__weights** (optional) - **T2**:
  weights to optimize.
* **__group_720__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_720__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_720__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_720__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_721__weights** (optional) - **T2**:
  weights to optimize.
* **__group_721__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_721__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_721__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_721__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_722__weights** (optional) - **T2**:
  weights to optimize.
* **__group_722__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_722__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_722__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_722__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_723__weights** (optional) - **T2**:
  weights to optimize.
* **__group_723__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_723__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_723__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_723__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_724__weights** (optional) - **T2**:
  weights to optimize.
* **__group_724__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_724__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_724__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_724__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_725__weights** (optional) - **T2**:
  weights to optimize.
* **__group_725__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_725__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_725__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_725__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_726__weights** (optional) - **T2**:
  weights to optimize.
* **__group_726__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_726__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_726__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_726__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_727__weights** (optional) - **T2**:
  weights to optimize.
* **__group_727__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_727__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_727__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_727__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_728__weights** (optional) - **T2**:
  weights to optimize.
* **__group_728__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_728__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_728__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_728__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_729__weights** (optional) - **T2**:
  weights to optimize.
* **__group_729__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_729__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_729__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_729__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_730__weights** (optional) - **T2**:
  weights to optimize.
* **__group_730__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_730__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_730__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_730__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_731__weights** (optional) - **T2**:
  weights to optimize.
* **__group_731__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_731__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_731__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_731__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_732__weights** (optional) - **T2**:
  weights to optimize.
* **__group_732__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_732__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_732__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_732__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_733__weights** (optional) - **T2**:
  weights to optimize.
* **__group_733__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_733__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_733__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_733__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_734__weights** (optional) - **T2**:
  weights to optimize.
* **__group_734__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_734__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_734__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_734__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_735__weights** (optional) - **T2**:
  weights to optimize.
* **__group_735__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_735__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_735__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_735__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_736__weights** (optional) - **T2**:
  weights to optimize.
* **__group_736__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_736__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_736__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_736__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_737__weights** (optional) - **T2**:
  weights to optimize.
* **__group_737__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_737__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_737__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_737__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_738__weights** (optional) - **T2**:
  weights to optimize.
* **__group_738__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_738__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_738__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_738__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_739__weights** (optional) - **T2**:
  weights to optimize.
* **__group_739__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_739__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_739__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_739__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_740__weights** (optional) - **T2**:
  weights to optimize.
* **__group_740__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_740__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_740__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_740__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_741__weights** (optional) - **T2**:
  weights to optimize.
* **__group_741__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_741__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_741__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_741__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_742__weights** (optional) - **T2**:
  weights to optimize.
* **__group_742__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_742__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_742__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_742__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_743__weights** (optional) - **T2**:
  weights to optimize.
* **__group_743__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_743__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_743__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_743__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_744__weights** (optional) - **T2**:
  weights to optimize.
* **__group_744__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_744__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_744__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_744__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_745__weights** (optional) - **T2**:
  weights to optimize.
* **__group_745__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_745__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_745__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_745__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_746__weights** (optional) - **T2**:
  weights to optimize.
* **__group_746__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_746__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_746__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_746__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_747__weights** (optional) - **T2**:
  weights to optimize.
* **__group_747__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_747__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_747__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_747__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_748__weights** (optional) - **T2**:
  weights to optimize.
* **__group_748__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_748__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_748__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_748__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_749__weights** (optional) - **T2**:
  weights to optimize.
* **__group_749__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_749__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_749__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_749__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_750__weights** (optional) - **T2**:
  weights to optimize.
* **__group_750__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_750__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_750__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_750__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_751__weights** (optional) - **T2**:
  weights to optimize.
* **__group_751__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_751__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_751__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_751__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_752__weights** (optional) - **T2**:
  weights to optimize.
* **__group_752__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_752__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_752__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_752__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_753__weights** (optional) - **T2**:
  weights to optimize.
* **__group_753__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_753__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_753__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_753__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_754__weights** (optional) - **T2**:
  weights to optimize.
* **__group_754__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_754__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_754__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_754__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_755__weights** (optional) - **T2**:
  weights to optimize.
* **__group_755__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_755__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_755__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_755__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_756__weights** (optional) - **T2**:
  weights to optimize.
* **__group_756__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_756__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_756__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_756__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_757__weights** (optional) - **T2**:
  weights to optimize.
* **__group_757__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_757__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_757__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_757__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_758__weights** (optional) - **T2**:
  weights to optimize.
* **__group_758__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_758__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_758__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_758__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_759__weights** (optional) - **T2**:
  weights to optimize.
* **__group_759__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_759__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_759__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_759__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_760__weights** (optional) - **T2**:
  weights to optimize.
* **__group_760__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_760__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_760__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_760__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_761__weights** (optional) - **T2**:
  weights to optimize.
* **__group_761__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_761__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_761__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_761__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_762__weights** (optional) - **T2**:
  weights to optimize.
* **__group_762__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_762__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_762__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_762__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_763__weights** (optional) - **T2**:
  weights to optimize.
* **__group_763__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_763__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_763__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_763__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_764__weights** (optional) - **T2**:
  weights to optimize.
* **__group_764__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_764__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_764__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_764__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_765__weights** (optional) - **T2**:
  weights to optimize.
* **__group_765__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_765__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_765__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_765__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_766__weights** (optional) - **T2**:
  weights to optimize.
* **__group_766__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_766__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_766__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_766__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_767__weights** (optional) - **T2**:
  weights to optimize.
* **__group_767__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_767__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_767__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_767__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_768__weights** (optional) - **T2**:
  weights to optimize.
* **__group_768__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_768__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_768__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_768__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_769__weights** (optional) - **T2**:
  weights to optimize.
* **__group_769__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_769__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_769__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_769__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_770__weights** (optional) - **T2**:
  weights to optimize.
* **__group_770__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_770__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_770__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_770__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_771__weights** (optional) - **T2**:
  weights to optimize.
* **__group_771__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_771__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_771__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_771__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_772__weights** (optional) - **T2**:
  weights to optimize.
* **__group_772__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_772__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_772__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_772__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_773__weights** (optional) - **T2**:
  weights to optimize.
* **__group_773__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_773__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_773__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_773__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_774__weights** (optional) - **T2**:
  weights to optimize.
* **__group_774__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_774__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_774__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_774__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_775__weights** (optional) - **T2**:
  weights to optimize.
* **__group_775__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_775__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_775__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_775__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_776__weights** (optional) - **T2**:
  weights to optimize.
* **__group_776__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_776__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_776__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_776__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_777__weights** (optional) - **T2**:
  weights to optimize.
* **__group_777__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_777__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_777__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_777__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_778__weights** (optional) - **T2**:
  weights to optimize.
* **__group_778__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_778__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_778__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_778__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_779__weights** (optional) - **T2**:
  weights to optimize.
* **__group_779__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_779__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_779__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_779__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_780__weights** (optional) - **T2**:
  weights to optimize.
* **__group_780__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_780__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_780__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_780__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_781__weights** (optional) - **T2**:
  weights to optimize.
* **__group_781__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_781__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_781__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_781__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_782__weights** (optional) - **T2**:
  weights to optimize.
* **__group_782__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_782__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_782__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_782__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_783__weights** (optional) - **T2**:
  weights to optimize.
* **__group_783__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_783__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_783__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_783__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_784__weights** (optional) - **T2**:
  weights to optimize.
* **__group_784__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_784__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_784__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_784__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_785__weights** (optional) - **T2**:
  weights to optimize.
* **__group_785__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_785__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_785__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_785__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_786__weights** (optional) - **T2**:
  weights to optimize.
* **__group_786__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_786__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_786__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_786__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_787__weights** (optional) - **T2**:
  weights to optimize.
* **__group_787__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_787__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_787__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_787__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_788__weights** (optional) - **T2**:
  weights to optimize.
* **__group_788__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_788__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_788__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_788__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_789__weights** (optional) - **T2**:
  weights to optimize.
* **__group_789__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_789__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_789__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_789__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_790__weights** (optional) - **T2**:
  weights to optimize.
* **__group_790__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_790__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_790__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_790__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_791__weights** (optional) - **T2**:
  weights to optimize.
* **__group_791__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_791__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_791__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_791__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_792__weights** (optional) - **T2**:
  weights to optimize.
* **__group_792__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_792__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_792__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_792__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_793__weights** (optional) - **T2**:
  weights to optimize.
* **__group_793__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_793__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_793__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_793__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_794__weights** (optional) - **T2**:
  weights to optimize.
* **__group_794__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_794__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_794__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_794__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_795__weights** (optional) - **T2**:
  weights to optimize.
* **__group_795__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_795__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_795__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_795__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_796__weights** (optional) - **T2**:
  weights to optimize.
* **__group_796__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_796__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_796__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_796__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_797__weights** (optional) - **T2**:
  weights to optimize.
* **__group_797__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_797__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_797__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_797__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_798__weights** (optional) - **T2**:
  weights to optimize.
* **__group_798__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_798__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_798__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_798__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_799__weights** (optional) - **T2**:
  weights to optimize.
* **__group_799__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_799__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_799__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_799__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_800__weights** (optional) - **T2**:
  weights to optimize.
* **__group_800__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_800__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_800__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_800__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_801__weights** (optional) - **T2**:
  weights to optimize.
* **__group_801__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_801__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_801__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_801__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_802__weights** (optional) - **T2**:
  weights to optimize.
* **__group_802__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_802__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_802__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_802__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_803__weights** (optional) - **T2**:
  weights to optimize.
* **__group_803__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_803__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_803__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_803__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_804__weights** (optional) - **T2**:
  weights to optimize.
* **__group_804__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_804__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_804__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_804__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_805__weights** (optional) - **T2**:
  weights to optimize.
* **__group_805__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_805__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_805__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_805__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_806__weights** (optional) - **T2**:
  weights to optimize.
* **__group_806__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_806__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_806__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_806__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_807__weights** (optional) - **T2**:
  weights to optimize.
* **__group_807__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_807__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_807__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_807__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_808__weights** (optional) - **T2**:
  weights to optimize.
* **__group_808__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_808__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_808__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_808__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_809__weights** (optional) - **T2**:
  weights to optimize.
* **__group_809__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_809__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_809__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_809__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_810__weights** (optional) - **T2**:
  weights to optimize.
* **__group_810__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_810__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_810__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_810__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_811__weights** (optional) - **T2**:
  weights to optimize.
* **__group_811__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_811__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_811__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_811__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_812__weights** (optional) - **T2**:
  weights to optimize.
* **__group_812__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_812__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_812__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_812__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_813__weights** (optional) - **T2**:
  weights to optimize.
* **__group_813__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_813__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_813__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_813__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_814__weights** (optional) - **T2**:
  weights to optimize.
* **__group_814__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_814__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_814__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_814__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_815__weights** (optional) - **T2**:
  weights to optimize.
* **__group_815__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_815__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_815__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_815__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_816__weights** (optional) - **T2**:
  weights to optimize.
* **__group_816__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_816__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_816__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_816__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_817__weights** (optional) - **T2**:
  weights to optimize.
* **__group_817__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_817__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_817__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_817__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_818__weights** (optional) - **T2**:
  weights to optimize.
* **__group_818__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_818__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_818__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_818__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_819__weights** (optional) - **T2**:
  weights to optimize.
* **__group_819__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_819__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_819__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_819__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_820__weights** (optional) - **T2**:
  weights to optimize.
* **__group_820__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_820__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_820__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_820__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_821__weights** (optional) - **T2**:
  weights to optimize.
* **__group_821__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_821__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_821__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_821__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_822__weights** (optional) - **T2**:
  weights to optimize.
* **__group_822__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_822__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_822__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_822__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_823__weights** (optional) - **T2**:
  weights to optimize.
* **__group_823__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_823__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_823__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_823__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_824__weights** (optional) - **T2**:
  weights to optimize.
* **__group_824__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_824__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_824__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_824__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_825__weights** (optional) - **T2**:
  weights to optimize.
* **__group_825__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_825__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_825__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_825__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_826__weights** (optional) - **T2**:
  weights to optimize.
* **__group_826__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_826__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_826__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_826__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_827__weights** (optional) - **T2**:
  weights to optimize.
* **__group_827__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_827__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_827__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_827__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_828__weights** (optional) - **T2**:
  weights to optimize.
* **__group_828__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_828__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_828__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_828__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_829__weights** (optional) - **T2**:
  weights to optimize.
* **__group_829__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_829__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_829__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_829__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_830__weights** (optional) - **T2**:
  weights to optimize.
* **__group_830__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_830__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_830__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_830__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_831__weights** (optional) - **T2**:
  weights to optimize.
* **__group_831__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_831__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_831__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_831__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_832__weights** (optional) - **T2**:
  weights to optimize.
* **__group_832__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_832__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_832__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_832__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_833__weights** (optional) - **T2**:
  weights to optimize.
* **__group_833__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_833__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_833__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_833__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_834__weights** (optional) - **T2**:
  weights to optimize.
* **__group_834__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_834__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_834__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_834__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_835__weights** (optional) - **T2**:
  weights to optimize.
* **__group_835__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_835__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_835__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_835__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_836__weights** (optional) - **T2**:
  weights to optimize.
* **__group_836__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_836__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_836__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_836__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_837__weights** (optional) - **T2**:
  weights to optimize.
* **__group_837__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_837__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_837__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_837__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_838__weights** (optional) - **T2**:
  weights to optimize.
* **__group_838__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_838__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_838__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_838__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_839__weights** (optional) - **T2**:
  weights to optimize.
* **__group_839__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_839__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_839__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_839__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_840__weights** (optional) - **T2**:
  weights to optimize.
* **__group_840__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_840__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_840__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_840__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_841__weights** (optional) - **T2**:
  weights to optimize.
* **__group_841__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_841__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_841__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_841__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_842__weights** (optional) - **T2**:
  weights to optimize.
* **__group_842__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_842__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_842__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_842__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_843__weights** (optional) - **T2**:
  weights to optimize.
* **__group_843__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_843__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_843__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_843__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_844__weights** (optional) - **T2**:
  weights to optimize.
* **__group_844__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_844__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_844__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_844__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_845__weights** (optional) - **T2**:
  weights to optimize.
* **__group_845__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_845__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_845__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_845__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_846__weights** (optional) - **T2**:
  weights to optimize.
* **__group_846__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_846__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_846__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_846__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_847__weights** (optional) - **T2**:
  weights to optimize.
* **__group_847__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_847__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_847__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_847__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_848__weights** (optional) - **T2**:
  weights to optimize.
* **__group_848__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_848__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_848__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_848__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_849__weights** (optional) - **T2**:
  weights to optimize.
* **__group_849__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_849__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_849__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_849__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_850__weights** (optional) - **T2**:
  weights to optimize.
* **__group_850__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_850__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_850__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_850__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_851__weights** (optional) - **T2**:
  weights to optimize.
* **__group_851__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_851__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_851__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_851__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_852__weights** (optional) - **T2**:
  weights to optimize.
* **__group_852__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_852__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_852__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_852__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_853__weights** (optional) - **T2**:
  weights to optimize.
* **__group_853__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_853__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_853__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_853__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_854__weights** (optional) - **T2**:
  weights to optimize.
* **__group_854__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_854__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_854__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_854__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_855__weights** (optional) - **T2**:
  weights to optimize.
* **__group_855__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_855__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_855__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_855__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_856__weights** (optional) - **T2**:
  weights to optimize.
* **__group_856__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_856__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_856__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_856__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_857__weights** (optional) - **T2**:
  weights to optimize.
* **__group_857__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_857__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_857__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_857__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_858__weights** (optional) - **T2**:
  weights to optimize.
* **__group_858__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_858__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_858__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_858__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_859__weights** (optional) - **T2**:
  weights to optimize.
* **__group_859__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_859__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_859__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_859__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_860__weights** (optional) - **T2**:
  weights to optimize.
* **__group_860__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_860__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_860__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_860__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_861__weights** (optional) - **T2**:
  weights to optimize.
* **__group_861__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_861__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_861__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_861__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_862__weights** (optional) - **T2**:
  weights to optimize.
* **__group_862__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_862__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_862__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_862__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_863__weights** (optional) - **T2**:
  weights to optimize.
* **__group_863__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_863__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_863__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_863__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_864__weights** (optional) - **T2**:
  weights to optimize.
* **__group_864__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_864__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_864__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_864__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_865__weights** (optional) - **T2**:
  weights to optimize.
* **__group_865__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_865__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_865__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_865__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_866__weights** (optional) - **T2**:
  weights to optimize.
* **__group_866__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_866__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_866__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_866__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_867__weights** (optional) - **T2**:
  weights to optimize.
* **__group_867__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_867__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_867__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_867__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_868__weights** (optional) - **T2**:
  weights to optimize.
* **__group_868__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_868__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_868__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_868__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_869__weights** (optional) - **T2**:
  weights to optimize.
* **__group_869__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_869__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_869__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_869__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_870__weights** (optional) - **T2**:
  weights to optimize.
* **__group_870__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_870__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_870__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_870__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_871__weights** (optional) - **T2**:
  weights to optimize.
* **__group_871__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_871__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_871__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_871__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_872__weights** (optional) - **T2**:
  weights to optimize.
* **__group_872__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_872__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_872__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_872__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_873__weights** (optional) - **T2**:
  weights to optimize.
* **__group_873__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_873__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_873__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_873__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_874__weights** (optional) - **T2**:
  weights to optimize.
* **__group_874__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_874__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_874__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_874__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_875__weights** (optional) - **T2**:
  weights to optimize.
* **__group_875__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_875__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_875__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_875__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_876__weights** (optional) - **T2**:
  weights to optimize.
* **__group_876__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_876__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_876__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_876__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_877__weights** (optional) - **T2**:
  weights to optimize.
* **__group_877__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_877__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_877__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_877__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_878__weights** (optional) - **T2**:
  weights to optimize.
* **__group_878__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_878__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_878__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_878__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_879__weights** (optional) - **T2**:
  weights to optimize.
* **__group_879__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_879__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_879__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_879__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_880__weights** (optional) - **T2**:
  weights to optimize.
* **__group_880__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_880__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_880__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_880__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_881__weights** (optional) - **T2**:
  weights to optimize.
* **__group_881__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_881__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_881__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_881__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_882__weights** (optional) - **T2**:
  weights to optimize.
* **__group_882__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_882__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_882__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_882__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_883__weights** (optional) - **T2**:
  weights to optimize.
* **__group_883__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_883__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_883__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_883__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_884__weights** (optional) - **T2**:
  weights to optimize.
* **__group_884__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_884__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_884__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_884__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_885__weights** (optional) - **T2**:
  weights to optimize.
* **__group_885__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_885__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_885__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_885__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_886__weights** (optional) - **T2**:
  weights to optimize.
* **__group_886__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_886__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_886__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_886__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_887__weights** (optional) - **T2**:
  weights to optimize.
* **__group_887__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_887__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_887__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_887__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_888__weights** (optional) - **T2**:
  weights to optimize.
* **__group_888__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_888__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_888__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_888__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_889__weights** (optional) - **T2**:
  weights to optimize.
* **__group_889__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_889__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_889__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_889__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_890__weights** (optional) - **T2**:
  weights to optimize.
* **__group_890__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_890__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_890__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_890__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_891__weights** (optional) - **T2**:
  weights to optimize.
* **__group_891__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_891__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_891__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_891__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_892__weights** (optional) - **T2**:
  weights to optimize.
* **__group_892__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_892__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_892__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_892__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_893__weights** (optional) - **T2**:
  weights to optimize.
* **__group_893__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_893__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_893__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_893__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_894__weights** (optional) - **T2**:
  weights to optimize.
* **__group_894__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_894__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_894__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_894__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_895__weights** (optional) - **T2**:
  weights to optimize.
* **__group_895__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_895__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_895__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_895__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_896__weights** (optional) - **T2**:
  weights to optimize.
* **__group_896__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_896__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_896__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_896__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_897__weights** (optional) - **T2**:
  weights to optimize.
* **__group_897__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_897__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_897__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_897__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_898__weights** (optional) - **T2**:
  weights to optimize.
* **__group_898__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_898__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_898__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_898__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_899__weights** (optional) - **T2**:
  weights to optimize.
* **__group_899__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_899__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_899__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_899__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_900__weights** (optional) - **T2**:
  weights to optimize.
* **__group_900__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_900__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_900__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_900__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_901__weights** (optional) - **T2**:
  weights to optimize.
* **__group_901__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_901__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_901__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_901__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_902__weights** (optional) - **T2**:
  weights to optimize.
* **__group_902__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_902__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_902__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_902__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_903__weights** (optional) - **T2**:
  weights to optimize.
* **__group_903__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_903__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_903__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_903__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_904__weights** (optional) - **T2**:
  weights to optimize.
* **__group_904__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_904__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_904__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_904__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_905__weights** (optional) - **T2**:
  weights to optimize.
* **__group_905__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_905__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_905__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_905__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_906__weights** (optional) - **T2**:
  weights to optimize.
* **__group_906__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_906__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_906__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_906__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_907__weights** (optional) - **T2**:
  weights to optimize.
* **__group_907__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_907__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_907__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_907__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_908__weights** (optional) - **T2**:
  weights to optimize.
* **__group_908__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_908__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_908__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_908__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_909__weights** (optional) - **T2**:
  weights to optimize.
* **__group_909__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_909__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_909__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_909__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_910__weights** (optional) - **T2**:
  weights to optimize.
* **__group_910__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_910__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_910__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_910__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_911__weights** (optional) - **T2**:
  weights to optimize.
* **__group_911__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_911__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_911__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_911__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_912__weights** (optional) - **T2**:
  weights to optimize.
* **__group_912__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_912__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_912__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_912__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_913__weights** (optional) - **T2**:
  weights to optimize.
* **__group_913__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_913__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_913__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_913__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_914__weights** (optional) - **T2**:
  weights to optimize.
* **__group_914__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_914__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_914__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_914__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_915__weights** (optional) - **T2**:
  weights to optimize.
* **__group_915__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_915__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_915__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_915__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_916__weights** (optional) - **T2**:
  weights to optimize.
* **__group_916__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_916__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_916__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_916__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_917__weights** (optional) - **T2**:
  weights to optimize.
* **__group_917__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_917__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_917__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_917__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_918__weights** (optional) - **T2**:
  weights to optimize.
* **__group_918__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_918__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_918__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_918__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_919__weights** (optional) - **T2**:
  weights to optimize.
* **__group_919__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_919__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_919__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_919__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_920__weights** (optional) - **T2**:
  weights to optimize.
* **__group_920__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_920__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_920__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_920__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_921__weights** (optional) - **T2**:
  weights to optimize.
* **__group_921__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_921__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_921__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_921__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_922__weights** (optional) - **T2**:
  weights to optimize.
* **__group_922__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_922__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_922__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_922__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_923__weights** (optional) - **T2**:
  weights to optimize.
* **__group_923__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_923__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_923__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_923__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_924__weights** (optional) - **T2**:
  weights to optimize.
* **__group_924__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_924__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_924__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_924__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_925__weights** (optional) - **T2**:
  weights to optimize.
* **__group_925__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_925__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_925__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_925__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_926__weights** (optional) - **T2**:
  weights to optimize.
* **__group_926__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_926__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_926__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_926__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_927__weights** (optional) - **T2**:
  weights to optimize.
* **__group_927__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_927__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_927__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_927__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_928__weights** (optional) - **T2**:
  weights to optimize.
* **__group_928__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_928__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_928__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_928__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_929__weights** (optional) - **T2**:
  weights to optimize.
* **__group_929__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_929__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_929__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_929__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_930__weights** (optional) - **T2**:
  weights to optimize.
* **__group_930__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_930__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_930__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_930__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_931__weights** (optional) - **T2**:
  weights to optimize.
* **__group_931__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_931__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_931__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_931__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_932__weights** (optional) - **T2**:
  weights to optimize.
* **__group_932__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_932__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_932__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_932__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_933__weights** (optional) - **T2**:
  weights to optimize.
* **__group_933__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_933__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_933__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_933__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_934__weights** (optional) - **T2**:
  weights to optimize.
* **__group_934__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_934__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_934__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_934__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_935__weights** (optional) - **T2**:
  weights to optimize.
* **__group_935__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_935__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_935__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_935__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_936__weights** (optional) - **T2**:
  weights to optimize.
* **__group_936__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_936__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_936__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_936__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_937__weights** (optional) - **T2**:
  weights to optimize.
* **__group_937__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_937__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_937__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_937__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_938__weights** (optional) - **T2**:
  weights to optimize.
* **__group_938__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_938__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_938__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_938__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_939__weights** (optional) - **T2**:
  weights to optimize.
* **__group_939__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_939__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_939__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_939__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_940__weights** (optional) - **T2**:
  weights to optimize.
* **__group_940__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_940__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_940__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_940__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_941__weights** (optional) - **T2**:
  weights to optimize.
* **__group_941__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_941__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_941__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_941__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_942__weights** (optional) - **T2**:
  weights to optimize.
* **__group_942__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_942__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_942__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_942__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_943__weights** (optional) - **T2**:
  weights to optimize.
* **__group_943__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_943__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_943__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_943__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_944__weights** (optional) - **T2**:
  weights to optimize.
* **__group_944__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_944__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_944__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_944__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_945__weights** (optional) - **T2**:
  weights to optimize.
* **__group_945__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_945__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_945__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_945__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_946__weights** (optional) - **T2**:
  weights to optimize.
* **__group_946__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_946__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_946__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_946__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_947__weights** (optional) - **T2**:
  weights to optimize.
* **__group_947__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_947__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_947__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_947__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_948__weights** (optional) - **T2**:
  weights to optimize.
* **__group_948__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_948__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_948__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_948__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_949__weights** (optional) - **T2**:
  weights to optimize.
* **__group_949__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_949__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_949__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_949__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_950__weights** (optional) - **T2**:
  weights to optimize.
* **__group_950__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_950__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_950__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_950__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_951__weights** (optional) - **T2**:
  weights to optimize.
* **__group_951__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_951__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_951__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_951__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_952__weights** (optional) - **T2**:
  weights to optimize.
* **__group_952__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_952__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_952__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_952__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_953__weights** (optional) - **T2**:
  weights to optimize.
* **__group_953__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_953__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_953__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_953__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_954__weights** (optional) - **T2**:
  weights to optimize.
* **__group_954__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_954__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_954__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_954__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_955__weights** (optional) - **T2**:
  weights to optimize.
* **__group_955__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_955__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_955__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_955__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_956__weights** (optional) - **T2**:
  weights to optimize.
* **__group_956__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_956__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_956__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_956__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_957__weights** (optional) - **T2**:
  weights to optimize.
* **__group_957__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_957__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_957__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_957__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_958__weights** (optional) - **T2**:
  weights to optimize.
* **__group_958__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_958__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_958__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_958__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_959__weights** (optional) - **T2**:
  weights to optimize.
* **__group_959__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_959__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_959__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_959__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_960__weights** (optional) - **T2**:
  weights to optimize.
* **__group_960__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_960__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_960__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_960__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_961__weights** (optional) - **T2**:
  weights to optimize.
* **__group_961__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_961__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_961__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_961__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_962__weights** (optional) - **T2**:
  weights to optimize.
* **__group_962__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_962__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_962__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_962__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_963__weights** (optional) - **T2**:
  weights to optimize.
* **__group_963__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_963__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_963__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_963__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_964__weights** (optional) - **T2**:
  weights to optimize.
* **__group_964__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_964__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_964__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_964__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_965__weights** (optional) - **T2**:
  weights to optimize.
* **__group_965__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_965__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_965__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_965__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_966__weights** (optional) - **T2**:
  weights to optimize.
* **__group_966__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_966__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_966__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_966__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_967__weights** (optional) - **T2**:
  weights to optimize.
* **__group_967__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_967__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_967__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_967__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_968__weights** (optional) - **T2**:
  weights to optimize.
* **__group_968__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_968__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_968__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_968__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_969__weights** (optional) - **T2**:
  weights to optimize.
* **__group_969__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_969__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_969__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_969__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_970__weights** (optional) - **T2**:
  weights to optimize.
* **__group_970__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_970__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_970__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_970__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_971__weights** (optional) - **T2**:
  weights to optimize.
* **__group_971__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_971__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_971__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_971__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_972__weights** (optional) - **T2**:
  weights to optimize.
* **__group_972__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_972__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_972__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_972__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_973__weights** (optional) - **T2**:
  weights to optimize.
* **__group_973__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_973__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_973__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_973__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_974__weights** (optional) - **T2**:
  weights to optimize.
* **__group_974__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_974__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_974__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_974__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_975__weights** (optional) - **T2**:
  weights to optimize.
* **__group_975__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_975__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_975__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_975__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_976__weights** (optional) - **T2**:
  weights to optimize.
* **__group_976__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_976__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_976__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_976__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_977__weights** (optional) - **T2**:
  weights to optimize.
* **__group_977__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_977__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_977__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_977__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_978__weights** (optional) - **T2**:
  weights to optimize.
* **__group_978__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_978__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_978__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_978__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_979__weights** (optional) - **T2**:
  weights to optimize.
* **__group_979__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_979__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_979__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_979__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_980__weights** (optional) - **T2**:
  weights to optimize.
* **__group_980__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_980__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_980__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_980__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_981__weights** (optional) - **T2**:
  weights to optimize.
* **__group_981__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_981__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_981__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_981__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_982__weights** (optional) - **T2**:
  weights to optimize.
* **__group_982__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_982__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_982__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_982__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_983__weights** (optional) - **T2**:
  weights to optimize.
* **__group_983__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_983__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_983__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_983__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_984__weights** (optional) - **T2**:
  weights to optimize.
* **__group_984__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_984__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_984__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_984__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_985__weights** (optional) - **T2**:
  weights to optimize.
* **__group_985__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_985__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_985__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_985__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_986__weights** (optional) - **T2**:
  weights to optimize.
* **__group_986__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_986__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_986__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_986__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_987__weights** (optional) - **T2**:
  weights to optimize.
* **__group_987__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_987__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_987__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_987__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_988__weights** (optional) - **T2**:
  weights to optimize.
* **__group_988__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_988__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_988__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_988__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_989__weights** (optional) - **T2**:
  weights to optimize.
* **__group_989__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_989__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_989__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_989__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_990__weights** (optional) - **T2**:
  weights to optimize.
* **__group_990__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_990__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_990__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_990__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_991__weights** (optional) - **T2**:
  weights to optimize.
* **__group_991__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_991__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_991__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_991__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_992__weights** (optional) - **T2**:
  weights to optimize.
* **__group_992__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_992__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_992__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_992__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_993__weights** (optional) - **T2**:
  weights to optimize.
* **__group_993__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_993__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_993__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_993__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_994__weights** (optional) - **T2**:
  weights to optimize.
* **__group_994__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_994__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_994__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_994__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_995__weights** (optional) - **T2**:
  weights to optimize.
* **__group_995__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_995__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_995__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_995__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_996__weights** (optional) - **T2**:
  weights to optimize.
* **__group_996__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_996__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_996__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_996__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_997__weights** (optional) - **T2**:
  weights to optimize.
* **__group_997__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_997__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_997__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_997__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_998__weights** (optional) - **T2**:
  weights to optimize.
* **__group_998__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_998__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_998__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_998__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_999__weights** (optional) - **T2**:
  weights to optimize.
* **__group_999__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_999__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_999__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_999__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1000__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1000__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1000__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1000__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1000__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1001__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1001__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1001__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1001__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1001__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1002__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1002__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1002__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1002__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1002__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1003__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1003__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1003__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1003__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1003__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1004__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1004__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1004__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1004__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1004__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1005__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1005__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1005__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1005__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1005__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1006__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1006__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1006__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1006__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1006__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1007__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1007__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1007__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1007__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1007__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1008__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1008__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1008__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1008__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1008__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1009__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1009__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1009__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1009__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1009__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1010__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1010__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1010__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1010__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1010__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1011__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1011__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1011__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1011__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1011__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1012__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1012__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1012__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1012__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1012__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1013__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1013__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1013__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1013__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1013__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1014__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1014__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1014__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1014__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1014__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1015__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1015__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1015__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1015__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1015__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1016__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1016__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1016__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1016__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1016__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1017__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1017__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1017__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1017__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1017__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1018__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1018__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1018__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1018__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1018__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1019__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1019__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1019__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1019__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1019__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1020__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1020__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1020__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1020__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1020__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1021__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1021__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1021__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1021__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1021__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1022__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1022__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1022__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1022__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1022__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.
* **__group_1023__weights** (optional) - **T2**:
  weights to optimize.
* **__group_1023__gradients** (optional) - **T3**:
  gradients computed in this iteration.
* **__group_1023__moment1** (optional) - **T4**:
  exponentially averaged historical gradients.
* **__group_1023__moment2** (optional) - **T4**:
  exponentially averaged historical squared gradients.
* **__group_1023__mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  FP16 or BF16 weights to optimize.

**Outputs**

Between 0 and 5121 outputs.

* **new_step** (optional, heterogeneous) - **TInt64**:
  One-based index of the next training iteration.
* **__group_0__new_weights** (optional) - **T2**:
  New weights
* **__group_0__new_gradients** (optional) - **T3**:
  New gradients
* **__group_0__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_0__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_0__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1__new_weights** (optional) - **T2**:
  New weights
* **__group_1__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_2__new_weights** (optional) - **T2**:
  New weights
* **__group_2__new_gradients** (optional) - **T3**:
  New gradients
* **__group_2__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_2__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_2__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_3__new_weights** (optional) - **T2**:
  New weights
* **__group_3__new_gradients** (optional) - **T3**:
  New gradients
* **__group_3__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_3__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_3__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_4__new_weights** (optional) - **T2**:
  New weights
* **__group_4__new_gradients** (optional) - **T3**:
  New gradients
* **__group_4__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_4__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_4__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_5__new_weights** (optional) - **T2**:
  New weights
* **__group_5__new_gradients** (optional) - **T3**:
  New gradients
* **__group_5__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_5__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_5__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_6__new_weights** (optional) - **T2**:
  New weights
* **__group_6__new_gradients** (optional) - **T3**:
  New gradients
* **__group_6__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_6__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_6__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_7__new_weights** (optional) - **T2**:
  New weights
* **__group_7__new_gradients** (optional) - **T3**:
  New gradients
* **__group_7__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_7__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_7__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_8__new_weights** (optional) - **T2**:
  New weights
* **__group_8__new_gradients** (optional) - **T3**:
  New gradients
* **__group_8__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_8__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_8__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_9__new_weights** (optional) - **T2**:
  New weights
* **__group_9__new_gradients** (optional) - **T3**:
  New gradients
* **__group_9__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_9__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_9__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_10__new_weights** (optional) - **T2**:
  New weights
* **__group_10__new_gradients** (optional) - **T3**:
  New gradients
* **__group_10__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_10__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_10__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_11__new_weights** (optional) - **T2**:
  New weights
* **__group_11__new_gradients** (optional) - **T3**:
  New gradients
* **__group_11__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_11__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_11__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_12__new_weights** (optional) - **T2**:
  New weights
* **__group_12__new_gradients** (optional) - **T3**:
  New gradients
* **__group_12__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_12__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_12__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_13__new_weights** (optional) - **T2**:
  New weights
* **__group_13__new_gradients** (optional) - **T3**:
  New gradients
* **__group_13__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_13__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_13__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_14__new_weights** (optional) - **T2**:
  New weights
* **__group_14__new_gradients** (optional) - **T3**:
  New gradients
* **__group_14__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_14__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_14__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_15__new_weights** (optional) - **T2**:
  New weights
* **__group_15__new_gradients** (optional) - **T3**:
  New gradients
* **__group_15__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_15__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_15__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_16__new_weights** (optional) - **T2**:
  New weights
* **__group_16__new_gradients** (optional) - **T3**:
  New gradients
* **__group_16__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_16__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_16__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_17__new_weights** (optional) - **T2**:
  New weights
* **__group_17__new_gradients** (optional) - **T3**:
  New gradients
* **__group_17__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_17__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_17__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_18__new_weights** (optional) - **T2**:
  New weights
* **__group_18__new_gradients** (optional) - **T3**:
  New gradients
* **__group_18__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_18__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_18__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_19__new_weights** (optional) - **T2**:
  New weights
* **__group_19__new_gradients** (optional) - **T3**:
  New gradients
* **__group_19__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_19__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_19__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_20__new_weights** (optional) - **T2**:
  New weights
* **__group_20__new_gradients** (optional) - **T3**:
  New gradients
* **__group_20__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_20__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_20__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_21__new_weights** (optional) - **T2**:
  New weights
* **__group_21__new_gradients** (optional) - **T3**:
  New gradients
* **__group_21__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_21__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_21__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_22__new_weights** (optional) - **T2**:
  New weights
* **__group_22__new_gradients** (optional) - **T3**:
  New gradients
* **__group_22__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_22__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_22__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_23__new_weights** (optional) - **T2**:
  New weights
* **__group_23__new_gradients** (optional) - **T3**:
  New gradients
* **__group_23__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_23__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_23__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_24__new_weights** (optional) - **T2**:
  New weights
* **__group_24__new_gradients** (optional) - **T3**:
  New gradients
* **__group_24__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_24__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_24__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_25__new_weights** (optional) - **T2**:
  New weights
* **__group_25__new_gradients** (optional) - **T3**:
  New gradients
* **__group_25__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_25__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_25__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_26__new_weights** (optional) - **T2**:
  New weights
* **__group_26__new_gradients** (optional) - **T3**:
  New gradients
* **__group_26__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_26__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_26__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_27__new_weights** (optional) - **T2**:
  New weights
* **__group_27__new_gradients** (optional) - **T3**:
  New gradients
* **__group_27__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_27__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_27__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_28__new_weights** (optional) - **T2**:
  New weights
* **__group_28__new_gradients** (optional) - **T3**:
  New gradients
* **__group_28__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_28__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_28__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_29__new_weights** (optional) - **T2**:
  New weights
* **__group_29__new_gradients** (optional) - **T3**:
  New gradients
* **__group_29__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_29__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_29__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_30__new_weights** (optional) - **T2**:
  New weights
* **__group_30__new_gradients** (optional) - **T3**:
  New gradients
* **__group_30__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_30__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_30__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_31__new_weights** (optional) - **T2**:
  New weights
* **__group_31__new_gradients** (optional) - **T3**:
  New gradients
* **__group_31__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_31__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_31__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_32__new_weights** (optional) - **T2**:
  New weights
* **__group_32__new_gradients** (optional) - **T3**:
  New gradients
* **__group_32__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_32__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_32__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_33__new_weights** (optional) - **T2**:
  New weights
* **__group_33__new_gradients** (optional) - **T3**:
  New gradients
* **__group_33__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_33__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_33__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_34__new_weights** (optional) - **T2**:
  New weights
* **__group_34__new_gradients** (optional) - **T3**:
  New gradients
* **__group_34__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_34__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_34__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_35__new_weights** (optional) - **T2**:
  New weights
* **__group_35__new_gradients** (optional) - **T3**:
  New gradients
* **__group_35__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_35__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_35__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_36__new_weights** (optional) - **T2**:
  New weights
* **__group_36__new_gradients** (optional) - **T3**:
  New gradients
* **__group_36__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_36__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_36__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_37__new_weights** (optional) - **T2**:
  New weights
* **__group_37__new_gradients** (optional) - **T3**:
  New gradients
* **__group_37__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_37__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_37__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_38__new_weights** (optional) - **T2**:
  New weights
* **__group_38__new_gradients** (optional) - **T3**:
  New gradients
* **__group_38__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_38__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_38__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_39__new_weights** (optional) - **T2**:
  New weights
* **__group_39__new_gradients** (optional) - **T3**:
  New gradients
* **__group_39__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_39__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_39__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_40__new_weights** (optional) - **T2**:
  New weights
* **__group_40__new_gradients** (optional) - **T3**:
  New gradients
* **__group_40__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_40__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_40__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_41__new_weights** (optional) - **T2**:
  New weights
* **__group_41__new_gradients** (optional) - **T3**:
  New gradients
* **__group_41__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_41__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_41__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_42__new_weights** (optional) - **T2**:
  New weights
* **__group_42__new_gradients** (optional) - **T3**:
  New gradients
* **__group_42__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_42__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_42__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_43__new_weights** (optional) - **T2**:
  New weights
* **__group_43__new_gradients** (optional) - **T3**:
  New gradients
* **__group_43__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_43__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_43__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_44__new_weights** (optional) - **T2**:
  New weights
* **__group_44__new_gradients** (optional) - **T3**:
  New gradients
* **__group_44__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_44__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_44__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_45__new_weights** (optional) - **T2**:
  New weights
* **__group_45__new_gradients** (optional) - **T3**:
  New gradients
* **__group_45__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_45__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_45__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_46__new_weights** (optional) - **T2**:
  New weights
* **__group_46__new_gradients** (optional) - **T3**:
  New gradients
* **__group_46__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_46__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_46__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_47__new_weights** (optional) - **T2**:
  New weights
* **__group_47__new_gradients** (optional) - **T3**:
  New gradients
* **__group_47__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_47__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_47__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_48__new_weights** (optional) - **T2**:
  New weights
* **__group_48__new_gradients** (optional) - **T3**:
  New gradients
* **__group_48__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_48__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_48__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_49__new_weights** (optional) - **T2**:
  New weights
* **__group_49__new_gradients** (optional) - **T3**:
  New gradients
* **__group_49__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_49__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_49__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_50__new_weights** (optional) - **T2**:
  New weights
* **__group_50__new_gradients** (optional) - **T3**:
  New gradients
* **__group_50__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_50__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_50__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_51__new_weights** (optional) - **T2**:
  New weights
* **__group_51__new_gradients** (optional) - **T3**:
  New gradients
* **__group_51__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_51__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_51__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_52__new_weights** (optional) - **T2**:
  New weights
* **__group_52__new_gradients** (optional) - **T3**:
  New gradients
* **__group_52__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_52__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_52__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_53__new_weights** (optional) - **T2**:
  New weights
* **__group_53__new_gradients** (optional) - **T3**:
  New gradients
* **__group_53__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_53__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_53__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_54__new_weights** (optional) - **T2**:
  New weights
* **__group_54__new_gradients** (optional) - **T3**:
  New gradients
* **__group_54__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_54__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_54__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_55__new_weights** (optional) - **T2**:
  New weights
* **__group_55__new_gradients** (optional) - **T3**:
  New gradients
* **__group_55__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_55__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_55__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_56__new_weights** (optional) - **T2**:
  New weights
* **__group_56__new_gradients** (optional) - **T3**:
  New gradients
* **__group_56__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_56__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_56__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_57__new_weights** (optional) - **T2**:
  New weights
* **__group_57__new_gradients** (optional) - **T3**:
  New gradients
* **__group_57__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_57__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_57__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_58__new_weights** (optional) - **T2**:
  New weights
* **__group_58__new_gradients** (optional) - **T3**:
  New gradients
* **__group_58__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_58__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_58__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_59__new_weights** (optional) - **T2**:
  New weights
* **__group_59__new_gradients** (optional) - **T3**:
  New gradients
* **__group_59__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_59__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_59__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_60__new_weights** (optional) - **T2**:
  New weights
* **__group_60__new_gradients** (optional) - **T3**:
  New gradients
* **__group_60__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_60__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_60__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_61__new_weights** (optional) - **T2**:
  New weights
* **__group_61__new_gradients** (optional) - **T3**:
  New gradients
* **__group_61__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_61__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_61__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_62__new_weights** (optional) - **T2**:
  New weights
* **__group_62__new_gradients** (optional) - **T3**:
  New gradients
* **__group_62__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_62__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_62__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_63__new_weights** (optional) - **T2**:
  New weights
* **__group_63__new_gradients** (optional) - **T3**:
  New gradients
* **__group_63__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_63__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_63__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_64__new_weights** (optional) - **T2**:
  New weights
* **__group_64__new_gradients** (optional) - **T3**:
  New gradients
* **__group_64__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_64__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_64__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_65__new_weights** (optional) - **T2**:
  New weights
* **__group_65__new_gradients** (optional) - **T3**:
  New gradients
* **__group_65__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_65__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_65__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_66__new_weights** (optional) - **T2**:
  New weights
* **__group_66__new_gradients** (optional) - **T3**:
  New gradients
* **__group_66__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_66__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_66__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_67__new_weights** (optional) - **T2**:
  New weights
* **__group_67__new_gradients** (optional) - **T3**:
  New gradients
* **__group_67__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_67__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_67__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_68__new_weights** (optional) - **T2**:
  New weights
* **__group_68__new_gradients** (optional) - **T3**:
  New gradients
* **__group_68__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_68__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_68__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_69__new_weights** (optional) - **T2**:
  New weights
* **__group_69__new_gradients** (optional) - **T3**:
  New gradients
* **__group_69__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_69__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_69__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_70__new_weights** (optional) - **T2**:
  New weights
* **__group_70__new_gradients** (optional) - **T3**:
  New gradients
* **__group_70__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_70__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_70__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_71__new_weights** (optional) - **T2**:
  New weights
* **__group_71__new_gradients** (optional) - **T3**:
  New gradients
* **__group_71__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_71__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_71__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_72__new_weights** (optional) - **T2**:
  New weights
* **__group_72__new_gradients** (optional) - **T3**:
  New gradients
* **__group_72__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_72__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_72__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_73__new_weights** (optional) - **T2**:
  New weights
* **__group_73__new_gradients** (optional) - **T3**:
  New gradients
* **__group_73__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_73__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_73__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_74__new_weights** (optional) - **T2**:
  New weights
* **__group_74__new_gradients** (optional) - **T3**:
  New gradients
* **__group_74__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_74__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_74__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_75__new_weights** (optional) - **T2**:
  New weights
* **__group_75__new_gradients** (optional) - **T3**:
  New gradients
* **__group_75__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_75__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_75__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_76__new_weights** (optional) - **T2**:
  New weights
* **__group_76__new_gradients** (optional) - **T3**:
  New gradients
* **__group_76__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_76__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_76__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_77__new_weights** (optional) - **T2**:
  New weights
* **__group_77__new_gradients** (optional) - **T3**:
  New gradients
* **__group_77__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_77__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_77__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_78__new_weights** (optional) - **T2**:
  New weights
* **__group_78__new_gradients** (optional) - **T3**:
  New gradients
* **__group_78__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_78__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_78__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_79__new_weights** (optional) - **T2**:
  New weights
* **__group_79__new_gradients** (optional) - **T3**:
  New gradients
* **__group_79__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_79__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_79__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_80__new_weights** (optional) - **T2**:
  New weights
* **__group_80__new_gradients** (optional) - **T3**:
  New gradients
* **__group_80__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_80__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_80__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_81__new_weights** (optional) - **T2**:
  New weights
* **__group_81__new_gradients** (optional) - **T3**:
  New gradients
* **__group_81__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_81__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_81__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_82__new_weights** (optional) - **T2**:
  New weights
* **__group_82__new_gradients** (optional) - **T3**:
  New gradients
* **__group_82__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_82__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_82__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_83__new_weights** (optional) - **T2**:
  New weights
* **__group_83__new_gradients** (optional) - **T3**:
  New gradients
* **__group_83__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_83__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_83__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_84__new_weights** (optional) - **T2**:
  New weights
* **__group_84__new_gradients** (optional) - **T3**:
  New gradients
* **__group_84__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_84__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_84__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_85__new_weights** (optional) - **T2**:
  New weights
* **__group_85__new_gradients** (optional) - **T3**:
  New gradients
* **__group_85__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_85__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_85__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_86__new_weights** (optional) - **T2**:
  New weights
* **__group_86__new_gradients** (optional) - **T3**:
  New gradients
* **__group_86__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_86__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_86__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_87__new_weights** (optional) - **T2**:
  New weights
* **__group_87__new_gradients** (optional) - **T3**:
  New gradients
* **__group_87__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_87__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_87__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_88__new_weights** (optional) - **T2**:
  New weights
* **__group_88__new_gradients** (optional) - **T3**:
  New gradients
* **__group_88__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_88__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_88__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_89__new_weights** (optional) - **T2**:
  New weights
* **__group_89__new_gradients** (optional) - **T3**:
  New gradients
* **__group_89__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_89__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_89__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_90__new_weights** (optional) - **T2**:
  New weights
* **__group_90__new_gradients** (optional) - **T3**:
  New gradients
* **__group_90__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_90__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_90__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_91__new_weights** (optional) - **T2**:
  New weights
* **__group_91__new_gradients** (optional) - **T3**:
  New gradients
* **__group_91__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_91__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_91__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_92__new_weights** (optional) - **T2**:
  New weights
* **__group_92__new_gradients** (optional) - **T3**:
  New gradients
* **__group_92__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_92__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_92__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_93__new_weights** (optional) - **T2**:
  New weights
* **__group_93__new_gradients** (optional) - **T3**:
  New gradients
* **__group_93__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_93__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_93__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_94__new_weights** (optional) - **T2**:
  New weights
* **__group_94__new_gradients** (optional) - **T3**:
  New gradients
* **__group_94__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_94__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_94__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_95__new_weights** (optional) - **T2**:
  New weights
* **__group_95__new_gradients** (optional) - **T3**:
  New gradients
* **__group_95__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_95__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_95__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_96__new_weights** (optional) - **T2**:
  New weights
* **__group_96__new_gradients** (optional) - **T3**:
  New gradients
* **__group_96__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_96__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_96__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_97__new_weights** (optional) - **T2**:
  New weights
* **__group_97__new_gradients** (optional) - **T3**:
  New gradients
* **__group_97__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_97__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_97__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_98__new_weights** (optional) - **T2**:
  New weights
* **__group_98__new_gradients** (optional) - **T3**:
  New gradients
* **__group_98__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_98__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_98__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_99__new_weights** (optional) - **T2**:
  New weights
* **__group_99__new_gradients** (optional) - **T3**:
  New gradients
* **__group_99__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_99__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_99__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_100__new_weights** (optional) - **T2**:
  New weights
* **__group_100__new_gradients** (optional) - **T3**:
  New gradients
* **__group_100__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_100__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_100__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_101__new_weights** (optional) - **T2**:
  New weights
* **__group_101__new_gradients** (optional) - **T3**:
  New gradients
* **__group_101__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_101__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_101__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_102__new_weights** (optional) - **T2**:
  New weights
* **__group_102__new_gradients** (optional) - **T3**:
  New gradients
* **__group_102__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_102__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_102__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_103__new_weights** (optional) - **T2**:
  New weights
* **__group_103__new_gradients** (optional) - **T3**:
  New gradients
* **__group_103__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_103__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_103__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_104__new_weights** (optional) - **T2**:
  New weights
* **__group_104__new_gradients** (optional) - **T3**:
  New gradients
* **__group_104__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_104__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_104__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_105__new_weights** (optional) - **T2**:
  New weights
* **__group_105__new_gradients** (optional) - **T3**:
  New gradients
* **__group_105__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_105__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_105__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_106__new_weights** (optional) - **T2**:
  New weights
* **__group_106__new_gradients** (optional) - **T3**:
  New gradients
* **__group_106__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_106__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_106__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_107__new_weights** (optional) - **T2**:
  New weights
* **__group_107__new_gradients** (optional) - **T3**:
  New gradients
* **__group_107__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_107__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_107__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_108__new_weights** (optional) - **T2**:
  New weights
* **__group_108__new_gradients** (optional) - **T3**:
  New gradients
* **__group_108__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_108__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_108__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_109__new_weights** (optional) - **T2**:
  New weights
* **__group_109__new_gradients** (optional) - **T3**:
  New gradients
* **__group_109__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_109__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_109__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_110__new_weights** (optional) - **T2**:
  New weights
* **__group_110__new_gradients** (optional) - **T3**:
  New gradients
* **__group_110__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_110__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_110__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_111__new_weights** (optional) - **T2**:
  New weights
* **__group_111__new_gradients** (optional) - **T3**:
  New gradients
* **__group_111__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_111__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_111__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_112__new_weights** (optional) - **T2**:
  New weights
* **__group_112__new_gradients** (optional) - **T3**:
  New gradients
* **__group_112__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_112__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_112__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_113__new_weights** (optional) - **T2**:
  New weights
* **__group_113__new_gradients** (optional) - **T3**:
  New gradients
* **__group_113__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_113__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_113__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_114__new_weights** (optional) - **T2**:
  New weights
* **__group_114__new_gradients** (optional) - **T3**:
  New gradients
* **__group_114__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_114__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_114__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_115__new_weights** (optional) - **T2**:
  New weights
* **__group_115__new_gradients** (optional) - **T3**:
  New gradients
* **__group_115__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_115__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_115__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_116__new_weights** (optional) - **T2**:
  New weights
* **__group_116__new_gradients** (optional) - **T3**:
  New gradients
* **__group_116__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_116__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_116__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_117__new_weights** (optional) - **T2**:
  New weights
* **__group_117__new_gradients** (optional) - **T3**:
  New gradients
* **__group_117__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_117__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_117__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_118__new_weights** (optional) - **T2**:
  New weights
* **__group_118__new_gradients** (optional) - **T3**:
  New gradients
* **__group_118__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_118__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_118__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_119__new_weights** (optional) - **T2**:
  New weights
* **__group_119__new_gradients** (optional) - **T3**:
  New gradients
* **__group_119__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_119__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_119__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_120__new_weights** (optional) - **T2**:
  New weights
* **__group_120__new_gradients** (optional) - **T3**:
  New gradients
* **__group_120__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_120__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_120__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_121__new_weights** (optional) - **T2**:
  New weights
* **__group_121__new_gradients** (optional) - **T3**:
  New gradients
* **__group_121__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_121__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_121__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_122__new_weights** (optional) - **T2**:
  New weights
* **__group_122__new_gradients** (optional) - **T3**:
  New gradients
* **__group_122__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_122__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_122__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_123__new_weights** (optional) - **T2**:
  New weights
* **__group_123__new_gradients** (optional) - **T3**:
  New gradients
* **__group_123__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_123__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_123__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_124__new_weights** (optional) - **T2**:
  New weights
* **__group_124__new_gradients** (optional) - **T3**:
  New gradients
* **__group_124__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_124__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_124__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_125__new_weights** (optional) - **T2**:
  New weights
* **__group_125__new_gradients** (optional) - **T3**:
  New gradients
* **__group_125__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_125__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_125__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_126__new_weights** (optional) - **T2**:
  New weights
* **__group_126__new_gradients** (optional) - **T3**:
  New gradients
* **__group_126__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_126__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_126__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_127__new_weights** (optional) - **T2**:
  New weights
* **__group_127__new_gradients** (optional) - **T3**:
  New gradients
* **__group_127__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_127__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_127__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_128__new_weights** (optional) - **T2**:
  New weights
* **__group_128__new_gradients** (optional) - **T3**:
  New gradients
* **__group_128__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_128__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_128__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_129__new_weights** (optional) - **T2**:
  New weights
* **__group_129__new_gradients** (optional) - **T3**:
  New gradients
* **__group_129__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_129__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_129__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_130__new_weights** (optional) - **T2**:
  New weights
* **__group_130__new_gradients** (optional) - **T3**:
  New gradients
* **__group_130__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_130__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_130__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_131__new_weights** (optional) - **T2**:
  New weights
* **__group_131__new_gradients** (optional) - **T3**:
  New gradients
* **__group_131__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_131__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_131__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_132__new_weights** (optional) - **T2**:
  New weights
* **__group_132__new_gradients** (optional) - **T3**:
  New gradients
* **__group_132__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_132__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_132__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_133__new_weights** (optional) - **T2**:
  New weights
* **__group_133__new_gradients** (optional) - **T3**:
  New gradients
* **__group_133__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_133__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_133__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_134__new_weights** (optional) - **T2**:
  New weights
* **__group_134__new_gradients** (optional) - **T3**:
  New gradients
* **__group_134__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_134__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_134__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_135__new_weights** (optional) - **T2**:
  New weights
* **__group_135__new_gradients** (optional) - **T3**:
  New gradients
* **__group_135__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_135__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_135__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_136__new_weights** (optional) - **T2**:
  New weights
* **__group_136__new_gradients** (optional) - **T3**:
  New gradients
* **__group_136__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_136__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_136__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_137__new_weights** (optional) - **T2**:
  New weights
* **__group_137__new_gradients** (optional) - **T3**:
  New gradients
* **__group_137__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_137__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_137__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_138__new_weights** (optional) - **T2**:
  New weights
* **__group_138__new_gradients** (optional) - **T3**:
  New gradients
* **__group_138__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_138__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_138__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_139__new_weights** (optional) - **T2**:
  New weights
* **__group_139__new_gradients** (optional) - **T3**:
  New gradients
* **__group_139__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_139__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_139__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_140__new_weights** (optional) - **T2**:
  New weights
* **__group_140__new_gradients** (optional) - **T3**:
  New gradients
* **__group_140__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_140__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_140__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_141__new_weights** (optional) - **T2**:
  New weights
* **__group_141__new_gradients** (optional) - **T3**:
  New gradients
* **__group_141__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_141__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_141__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_142__new_weights** (optional) - **T2**:
  New weights
* **__group_142__new_gradients** (optional) - **T3**:
  New gradients
* **__group_142__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_142__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_142__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_143__new_weights** (optional) - **T2**:
  New weights
* **__group_143__new_gradients** (optional) - **T3**:
  New gradients
* **__group_143__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_143__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_143__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_144__new_weights** (optional) - **T2**:
  New weights
* **__group_144__new_gradients** (optional) - **T3**:
  New gradients
* **__group_144__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_144__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_144__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_145__new_weights** (optional) - **T2**:
  New weights
* **__group_145__new_gradients** (optional) - **T3**:
  New gradients
* **__group_145__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_145__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_145__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_146__new_weights** (optional) - **T2**:
  New weights
* **__group_146__new_gradients** (optional) - **T3**:
  New gradients
* **__group_146__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_146__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_146__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_147__new_weights** (optional) - **T2**:
  New weights
* **__group_147__new_gradients** (optional) - **T3**:
  New gradients
* **__group_147__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_147__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_147__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_148__new_weights** (optional) - **T2**:
  New weights
* **__group_148__new_gradients** (optional) - **T3**:
  New gradients
* **__group_148__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_148__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_148__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_149__new_weights** (optional) - **T2**:
  New weights
* **__group_149__new_gradients** (optional) - **T3**:
  New gradients
* **__group_149__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_149__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_149__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_150__new_weights** (optional) - **T2**:
  New weights
* **__group_150__new_gradients** (optional) - **T3**:
  New gradients
* **__group_150__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_150__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_150__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_151__new_weights** (optional) - **T2**:
  New weights
* **__group_151__new_gradients** (optional) - **T3**:
  New gradients
* **__group_151__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_151__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_151__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_152__new_weights** (optional) - **T2**:
  New weights
* **__group_152__new_gradients** (optional) - **T3**:
  New gradients
* **__group_152__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_152__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_152__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_153__new_weights** (optional) - **T2**:
  New weights
* **__group_153__new_gradients** (optional) - **T3**:
  New gradients
* **__group_153__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_153__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_153__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_154__new_weights** (optional) - **T2**:
  New weights
* **__group_154__new_gradients** (optional) - **T3**:
  New gradients
* **__group_154__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_154__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_154__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_155__new_weights** (optional) - **T2**:
  New weights
* **__group_155__new_gradients** (optional) - **T3**:
  New gradients
* **__group_155__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_155__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_155__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_156__new_weights** (optional) - **T2**:
  New weights
* **__group_156__new_gradients** (optional) - **T3**:
  New gradients
* **__group_156__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_156__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_156__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_157__new_weights** (optional) - **T2**:
  New weights
* **__group_157__new_gradients** (optional) - **T3**:
  New gradients
* **__group_157__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_157__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_157__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_158__new_weights** (optional) - **T2**:
  New weights
* **__group_158__new_gradients** (optional) - **T3**:
  New gradients
* **__group_158__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_158__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_158__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_159__new_weights** (optional) - **T2**:
  New weights
* **__group_159__new_gradients** (optional) - **T3**:
  New gradients
* **__group_159__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_159__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_159__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_160__new_weights** (optional) - **T2**:
  New weights
* **__group_160__new_gradients** (optional) - **T3**:
  New gradients
* **__group_160__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_160__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_160__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_161__new_weights** (optional) - **T2**:
  New weights
* **__group_161__new_gradients** (optional) - **T3**:
  New gradients
* **__group_161__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_161__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_161__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_162__new_weights** (optional) - **T2**:
  New weights
* **__group_162__new_gradients** (optional) - **T3**:
  New gradients
* **__group_162__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_162__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_162__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_163__new_weights** (optional) - **T2**:
  New weights
* **__group_163__new_gradients** (optional) - **T3**:
  New gradients
* **__group_163__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_163__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_163__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_164__new_weights** (optional) - **T2**:
  New weights
* **__group_164__new_gradients** (optional) - **T3**:
  New gradients
* **__group_164__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_164__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_164__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_165__new_weights** (optional) - **T2**:
  New weights
* **__group_165__new_gradients** (optional) - **T3**:
  New gradients
* **__group_165__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_165__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_165__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_166__new_weights** (optional) - **T2**:
  New weights
* **__group_166__new_gradients** (optional) - **T3**:
  New gradients
* **__group_166__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_166__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_166__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_167__new_weights** (optional) - **T2**:
  New weights
* **__group_167__new_gradients** (optional) - **T3**:
  New gradients
* **__group_167__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_167__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_167__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_168__new_weights** (optional) - **T2**:
  New weights
* **__group_168__new_gradients** (optional) - **T3**:
  New gradients
* **__group_168__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_168__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_168__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_169__new_weights** (optional) - **T2**:
  New weights
* **__group_169__new_gradients** (optional) - **T3**:
  New gradients
* **__group_169__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_169__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_169__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_170__new_weights** (optional) - **T2**:
  New weights
* **__group_170__new_gradients** (optional) - **T3**:
  New gradients
* **__group_170__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_170__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_170__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_171__new_weights** (optional) - **T2**:
  New weights
* **__group_171__new_gradients** (optional) - **T3**:
  New gradients
* **__group_171__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_171__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_171__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_172__new_weights** (optional) - **T2**:
  New weights
* **__group_172__new_gradients** (optional) - **T3**:
  New gradients
* **__group_172__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_172__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_172__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_173__new_weights** (optional) - **T2**:
  New weights
* **__group_173__new_gradients** (optional) - **T3**:
  New gradients
* **__group_173__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_173__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_173__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_174__new_weights** (optional) - **T2**:
  New weights
* **__group_174__new_gradients** (optional) - **T3**:
  New gradients
* **__group_174__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_174__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_174__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_175__new_weights** (optional) - **T2**:
  New weights
* **__group_175__new_gradients** (optional) - **T3**:
  New gradients
* **__group_175__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_175__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_175__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_176__new_weights** (optional) - **T2**:
  New weights
* **__group_176__new_gradients** (optional) - **T3**:
  New gradients
* **__group_176__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_176__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_176__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_177__new_weights** (optional) - **T2**:
  New weights
* **__group_177__new_gradients** (optional) - **T3**:
  New gradients
* **__group_177__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_177__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_177__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_178__new_weights** (optional) - **T2**:
  New weights
* **__group_178__new_gradients** (optional) - **T3**:
  New gradients
* **__group_178__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_178__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_178__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_179__new_weights** (optional) - **T2**:
  New weights
* **__group_179__new_gradients** (optional) - **T3**:
  New gradients
* **__group_179__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_179__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_179__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_180__new_weights** (optional) - **T2**:
  New weights
* **__group_180__new_gradients** (optional) - **T3**:
  New gradients
* **__group_180__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_180__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_180__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_181__new_weights** (optional) - **T2**:
  New weights
* **__group_181__new_gradients** (optional) - **T3**:
  New gradients
* **__group_181__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_181__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_181__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_182__new_weights** (optional) - **T2**:
  New weights
* **__group_182__new_gradients** (optional) - **T3**:
  New gradients
* **__group_182__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_182__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_182__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_183__new_weights** (optional) - **T2**:
  New weights
* **__group_183__new_gradients** (optional) - **T3**:
  New gradients
* **__group_183__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_183__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_183__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_184__new_weights** (optional) - **T2**:
  New weights
* **__group_184__new_gradients** (optional) - **T3**:
  New gradients
* **__group_184__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_184__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_184__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_185__new_weights** (optional) - **T2**:
  New weights
* **__group_185__new_gradients** (optional) - **T3**:
  New gradients
* **__group_185__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_185__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_185__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_186__new_weights** (optional) - **T2**:
  New weights
* **__group_186__new_gradients** (optional) - **T3**:
  New gradients
* **__group_186__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_186__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_186__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_187__new_weights** (optional) - **T2**:
  New weights
* **__group_187__new_gradients** (optional) - **T3**:
  New gradients
* **__group_187__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_187__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_187__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_188__new_weights** (optional) - **T2**:
  New weights
* **__group_188__new_gradients** (optional) - **T3**:
  New gradients
* **__group_188__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_188__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_188__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_189__new_weights** (optional) - **T2**:
  New weights
* **__group_189__new_gradients** (optional) - **T3**:
  New gradients
* **__group_189__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_189__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_189__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_190__new_weights** (optional) - **T2**:
  New weights
* **__group_190__new_gradients** (optional) - **T3**:
  New gradients
* **__group_190__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_190__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_190__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_191__new_weights** (optional) - **T2**:
  New weights
* **__group_191__new_gradients** (optional) - **T3**:
  New gradients
* **__group_191__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_191__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_191__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_192__new_weights** (optional) - **T2**:
  New weights
* **__group_192__new_gradients** (optional) - **T3**:
  New gradients
* **__group_192__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_192__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_192__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_193__new_weights** (optional) - **T2**:
  New weights
* **__group_193__new_gradients** (optional) - **T3**:
  New gradients
* **__group_193__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_193__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_193__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_194__new_weights** (optional) - **T2**:
  New weights
* **__group_194__new_gradients** (optional) - **T3**:
  New gradients
* **__group_194__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_194__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_194__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_195__new_weights** (optional) - **T2**:
  New weights
* **__group_195__new_gradients** (optional) - **T3**:
  New gradients
* **__group_195__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_195__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_195__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_196__new_weights** (optional) - **T2**:
  New weights
* **__group_196__new_gradients** (optional) - **T3**:
  New gradients
* **__group_196__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_196__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_196__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_197__new_weights** (optional) - **T2**:
  New weights
* **__group_197__new_gradients** (optional) - **T3**:
  New gradients
* **__group_197__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_197__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_197__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_198__new_weights** (optional) - **T2**:
  New weights
* **__group_198__new_gradients** (optional) - **T3**:
  New gradients
* **__group_198__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_198__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_198__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_199__new_weights** (optional) - **T2**:
  New weights
* **__group_199__new_gradients** (optional) - **T3**:
  New gradients
* **__group_199__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_199__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_199__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_200__new_weights** (optional) - **T2**:
  New weights
* **__group_200__new_gradients** (optional) - **T3**:
  New gradients
* **__group_200__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_200__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_200__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_201__new_weights** (optional) - **T2**:
  New weights
* **__group_201__new_gradients** (optional) - **T3**:
  New gradients
* **__group_201__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_201__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_201__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_202__new_weights** (optional) - **T2**:
  New weights
* **__group_202__new_gradients** (optional) - **T3**:
  New gradients
* **__group_202__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_202__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_202__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_203__new_weights** (optional) - **T2**:
  New weights
* **__group_203__new_gradients** (optional) - **T3**:
  New gradients
* **__group_203__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_203__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_203__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_204__new_weights** (optional) - **T2**:
  New weights
* **__group_204__new_gradients** (optional) - **T3**:
  New gradients
* **__group_204__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_204__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_204__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_205__new_weights** (optional) - **T2**:
  New weights
* **__group_205__new_gradients** (optional) - **T3**:
  New gradients
* **__group_205__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_205__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_205__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_206__new_weights** (optional) - **T2**:
  New weights
* **__group_206__new_gradients** (optional) - **T3**:
  New gradients
* **__group_206__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_206__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_206__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_207__new_weights** (optional) - **T2**:
  New weights
* **__group_207__new_gradients** (optional) - **T3**:
  New gradients
* **__group_207__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_207__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_207__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_208__new_weights** (optional) - **T2**:
  New weights
* **__group_208__new_gradients** (optional) - **T3**:
  New gradients
* **__group_208__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_208__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_208__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_209__new_weights** (optional) - **T2**:
  New weights
* **__group_209__new_gradients** (optional) - **T3**:
  New gradients
* **__group_209__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_209__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_209__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_210__new_weights** (optional) - **T2**:
  New weights
* **__group_210__new_gradients** (optional) - **T3**:
  New gradients
* **__group_210__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_210__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_210__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_211__new_weights** (optional) - **T2**:
  New weights
* **__group_211__new_gradients** (optional) - **T3**:
  New gradients
* **__group_211__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_211__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_211__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_212__new_weights** (optional) - **T2**:
  New weights
* **__group_212__new_gradients** (optional) - **T3**:
  New gradients
* **__group_212__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_212__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_212__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_213__new_weights** (optional) - **T2**:
  New weights
* **__group_213__new_gradients** (optional) - **T3**:
  New gradients
* **__group_213__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_213__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_213__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_214__new_weights** (optional) - **T2**:
  New weights
* **__group_214__new_gradients** (optional) - **T3**:
  New gradients
* **__group_214__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_214__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_214__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_215__new_weights** (optional) - **T2**:
  New weights
* **__group_215__new_gradients** (optional) - **T3**:
  New gradients
* **__group_215__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_215__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_215__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_216__new_weights** (optional) - **T2**:
  New weights
* **__group_216__new_gradients** (optional) - **T3**:
  New gradients
* **__group_216__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_216__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_216__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_217__new_weights** (optional) - **T2**:
  New weights
* **__group_217__new_gradients** (optional) - **T3**:
  New gradients
* **__group_217__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_217__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_217__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_218__new_weights** (optional) - **T2**:
  New weights
* **__group_218__new_gradients** (optional) - **T3**:
  New gradients
* **__group_218__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_218__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_218__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_219__new_weights** (optional) - **T2**:
  New weights
* **__group_219__new_gradients** (optional) - **T3**:
  New gradients
* **__group_219__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_219__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_219__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_220__new_weights** (optional) - **T2**:
  New weights
* **__group_220__new_gradients** (optional) - **T3**:
  New gradients
* **__group_220__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_220__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_220__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_221__new_weights** (optional) - **T2**:
  New weights
* **__group_221__new_gradients** (optional) - **T3**:
  New gradients
* **__group_221__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_221__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_221__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_222__new_weights** (optional) - **T2**:
  New weights
* **__group_222__new_gradients** (optional) - **T3**:
  New gradients
* **__group_222__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_222__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_222__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_223__new_weights** (optional) - **T2**:
  New weights
* **__group_223__new_gradients** (optional) - **T3**:
  New gradients
* **__group_223__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_223__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_223__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_224__new_weights** (optional) - **T2**:
  New weights
* **__group_224__new_gradients** (optional) - **T3**:
  New gradients
* **__group_224__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_224__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_224__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_225__new_weights** (optional) - **T2**:
  New weights
* **__group_225__new_gradients** (optional) - **T3**:
  New gradients
* **__group_225__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_225__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_225__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_226__new_weights** (optional) - **T2**:
  New weights
* **__group_226__new_gradients** (optional) - **T3**:
  New gradients
* **__group_226__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_226__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_226__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_227__new_weights** (optional) - **T2**:
  New weights
* **__group_227__new_gradients** (optional) - **T3**:
  New gradients
* **__group_227__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_227__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_227__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_228__new_weights** (optional) - **T2**:
  New weights
* **__group_228__new_gradients** (optional) - **T3**:
  New gradients
* **__group_228__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_228__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_228__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_229__new_weights** (optional) - **T2**:
  New weights
* **__group_229__new_gradients** (optional) - **T3**:
  New gradients
* **__group_229__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_229__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_229__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_230__new_weights** (optional) - **T2**:
  New weights
* **__group_230__new_gradients** (optional) - **T3**:
  New gradients
* **__group_230__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_230__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_230__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_231__new_weights** (optional) - **T2**:
  New weights
* **__group_231__new_gradients** (optional) - **T3**:
  New gradients
* **__group_231__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_231__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_231__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_232__new_weights** (optional) - **T2**:
  New weights
* **__group_232__new_gradients** (optional) - **T3**:
  New gradients
* **__group_232__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_232__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_232__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_233__new_weights** (optional) - **T2**:
  New weights
* **__group_233__new_gradients** (optional) - **T3**:
  New gradients
* **__group_233__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_233__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_233__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_234__new_weights** (optional) - **T2**:
  New weights
* **__group_234__new_gradients** (optional) - **T3**:
  New gradients
* **__group_234__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_234__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_234__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_235__new_weights** (optional) - **T2**:
  New weights
* **__group_235__new_gradients** (optional) - **T3**:
  New gradients
* **__group_235__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_235__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_235__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_236__new_weights** (optional) - **T2**:
  New weights
* **__group_236__new_gradients** (optional) - **T3**:
  New gradients
* **__group_236__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_236__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_236__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_237__new_weights** (optional) - **T2**:
  New weights
* **__group_237__new_gradients** (optional) - **T3**:
  New gradients
* **__group_237__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_237__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_237__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_238__new_weights** (optional) - **T2**:
  New weights
* **__group_238__new_gradients** (optional) - **T3**:
  New gradients
* **__group_238__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_238__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_238__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_239__new_weights** (optional) - **T2**:
  New weights
* **__group_239__new_gradients** (optional) - **T3**:
  New gradients
* **__group_239__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_239__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_239__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_240__new_weights** (optional) - **T2**:
  New weights
* **__group_240__new_gradients** (optional) - **T3**:
  New gradients
* **__group_240__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_240__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_240__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_241__new_weights** (optional) - **T2**:
  New weights
* **__group_241__new_gradients** (optional) - **T3**:
  New gradients
* **__group_241__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_241__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_241__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_242__new_weights** (optional) - **T2**:
  New weights
* **__group_242__new_gradients** (optional) - **T3**:
  New gradients
* **__group_242__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_242__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_242__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_243__new_weights** (optional) - **T2**:
  New weights
* **__group_243__new_gradients** (optional) - **T3**:
  New gradients
* **__group_243__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_243__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_243__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_244__new_weights** (optional) - **T2**:
  New weights
* **__group_244__new_gradients** (optional) - **T3**:
  New gradients
* **__group_244__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_244__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_244__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_245__new_weights** (optional) - **T2**:
  New weights
* **__group_245__new_gradients** (optional) - **T3**:
  New gradients
* **__group_245__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_245__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_245__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_246__new_weights** (optional) - **T2**:
  New weights
* **__group_246__new_gradients** (optional) - **T3**:
  New gradients
* **__group_246__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_246__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_246__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_247__new_weights** (optional) - **T2**:
  New weights
* **__group_247__new_gradients** (optional) - **T3**:
  New gradients
* **__group_247__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_247__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_247__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_248__new_weights** (optional) - **T2**:
  New weights
* **__group_248__new_gradients** (optional) - **T3**:
  New gradients
* **__group_248__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_248__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_248__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_249__new_weights** (optional) - **T2**:
  New weights
* **__group_249__new_gradients** (optional) - **T3**:
  New gradients
* **__group_249__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_249__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_249__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_250__new_weights** (optional) - **T2**:
  New weights
* **__group_250__new_gradients** (optional) - **T3**:
  New gradients
* **__group_250__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_250__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_250__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_251__new_weights** (optional) - **T2**:
  New weights
* **__group_251__new_gradients** (optional) - **T3**:
  New gradients
* **__group_251__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_251__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_251__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_252__new_weights** (optional) - **T2**:
  New weights
* **__group_252__new_gradients** (optional) - **T3**:
  New gradients
* **__group_252__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_252__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_252__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_253__new_weights** (optional) - **T2**:
  New weights
* **__group_253__new_gradients** (optional) - **T3**:
  New gradients
* **__group_253__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_253__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_253__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_254__new_weights** (optional) - **T2**:
  New weights
* **__group_254__new_gradients** (optional) - **T3**:
  New gradients
* **__group_254__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_254__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_254__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_255__new_weights** (optional) - **T2**:
  New weights
* **__group_255__new_gradients** (optional) - **T3**:
  New gradients
* **__group_255__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_255__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_255__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_256__new_weights** (optional) - **T2**:
  New weights
* **__group_256__new_gradients** (optional) - **T3**:
  New gradients
* **__group_256__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_256__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_256__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_257__new_weights** (optional) - **T2**:
  New weights
* **__group_257__new_gradients** (optional) - **T3**:
  New gradients
* **__group_257__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_257__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_257__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_258__new_weights** (optional) - **T2**:
  New weights
* **__group_258__new_gradients** (optional) - **T3**:
  New gradients
* **__group_258__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_258__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_258__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_259__new_weights** (optional) - **T2**:
  New weights
* **__group_259__new_gradients** (optional) - **T3**:
  New gradients
* **__group_259__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_259__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_259__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_260__new_weights** (optional) - **T2**:
  New weights
* **__group_260__new_gradients** (optional) - **T3**:
  New gradients
* **__group_260__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_260__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_260__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_261__new_weights** (optional) - **T2**:
  New weights
* **__group_261__new_gradients** (optional) - **T3**:
  New gradients
* **__group_261__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_261__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_261__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_262__new_weights** (optional) - **T2**:
  New weights
* **__group_262__new_gradients** (optional) - **T3**:
  New gradients
* **__group_262__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_262__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_262__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_263__new_weights** (optional) - **T2**:
  New weights
* **__group_263__new_gradients** (optional) - **T3**:
  New gradients
* **__group_263__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_263__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_263__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_264__new_weights** (optional) - **T2**:
  New weights
* **__group_264__new_gradients** (optional) - **T3**:
  New gradients
* **__group_264__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_264__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_264__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_265__new_weights** (optional) - **T2**:
  New weights
* **__group_265__new_gradients** (optional) - **T3**:
  New gradients
* **__group_265__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_265__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_265__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_266__new_weights** (optional) - **T2**:
  New weights
* **__group_266__new_gradients** (optional) - **T3**:
  New gradients
* **__group_266__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_266__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_266__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_267__new_weights** (optional) - **T2**:
  New weights
* **__group_267__new_gradients** (optional) - **T3**:
  New gradients
* **__group_267__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_267__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_267__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_268__new_weights** (optional) - **T2**:
  New weights
* **__group_268__new_gradients** (optional) - **T3**:
  New gradients
* **__group_268__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_268__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_268__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_269__new_weights** (optional) - **T2**:
  New weights
* **__group_269__new_gradients** (optional) - **T3**:
  New gradients
* **__group_269__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_269__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_269__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_270__new_weights** (optional) - **T2**:
  New weights
* **__group_270__new_gradients** (optional) - **T3**:
  New gradients
* **__group_270__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_270__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_270__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_271__new_weights** (optional) - **T2**:
  New weights
* **__group_271__new_gradients** (optional) - **T3**:
  New gradients
* **__group_271__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_271__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_271__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_272__new_weights** (optional) - **T2**:
  New weights
* **__group_272__new_gradients** (optional) - **T3**:
  New gradients
* **__group_272__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_272__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_272__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_273__new_weights** (optional) - **T2**:
  New weights
* **__group_273__new_gradients** (optional) - **T3**:
  New gradients
* **__group_273__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_273__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_273__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_274__new_weights** (optional) - **T2**:
  New weights
* **__group_274__new_gradients** (optional) - **T3**:
  New gradients
* **__group_274__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_274__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_274__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_275__new_weights** (optional) - **T2**:
  New weights
* **__group_275__new_gradients** (optional) - **T3**:
  New gradients
* **__group_275__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_275__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_275__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_276__new_weights** (optional) - **T2**:
  New weights
* **__group_276__new_gradients** (optional) - **T3**:
  New gradients
* **__group_276__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_276__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_276__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_277__new_weights** (optional) - **T2**:
  New weights
* **__group_277__new_gradients** (optional) - **T3**:
  New gradients
* **__group_277__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_277__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_277__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_278__new_weights** (optional) - **T2**:
  New weights
* **__group_278__new_gradients** (optional) - **T3**:
  New gradients
* **__group_278__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_278__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_278__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_279__new_weights** (optional) - **T2**:
  New weights
* **__group_279__new_gradients** (optional) - **T3**:
  New gradients
* **__group_279__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_279__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_279__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_280__new_weights** (optional) - **T2**:
  New weights
* **__group_280__new_gradients** (optional) - **T3**:
  New gradients
* **__group_280__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_280__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_280__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_281__new_weights** (optional) - **T2**:
  New weights
* **__group_281__new_gradients** (optional) - **T3**:
  New gradients
* **__group_281__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_281__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_281__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_282__new_weights** (optional) - **T2**:
  New weights
* **__group_282__new_gradients** (optional) - **T3**:
  New gradients
* **__group_282__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_282__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_282__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_283__new_weights** (optional) - **T2**:
  New weights
* **__group_283__new_gradients** (optional) - **T3**:
  New gradients
* **__group_283__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_283__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_283__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_284__new_weights** (optional) - **T2**:
  New weights
* **__group_284__new_gradients** (optional) - **T3**:
  New gradients
* **__group_284__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_284__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_284__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_285__new_weights** (optional) - **T2**:
  New weights
* **__group_285__new_gradients** (optional) - **T3**:
  New gradients
* **__group_285__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_285__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_285__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_286__new_weights** (optional) - **T2**:
  New weights
* **__group_286__new_gradients** (optional) - **T3**:
  New gradients
* **__group_286__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_286__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_286__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_287__new_weights** (optional) - **T2**:
  New weights
* **__group_287__new_gradients** (optional) - **T3**:
  New gradients
* **__group_287__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_287__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_287__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_288__new_weights** (optional) - **T2**:
  New weights
* **__group_288__new_gradients** (optional) - **T3**:
  New gradients
* **__group_288__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_288__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_288__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_289__new_weights** (optional) - **T2**:
  New weights
* **__group_289__new_gradients** (optional) - **T3**:
  New gradients
* **__group_289__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_289__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_289__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_290__new_weights** (optional) - **T2**:
  New weights
* **__group_290__new_gradients** (optional) - **T3**:
  New gradients
* **__group_290__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_290__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_290__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_291__new_weights** (optional) - **T2**:
  New weights
* **__group_291__new_gradients** (optional) - **T3**:
  New gradients
* **__group_291__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_291__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_291__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_292__new_weights** (optional) - **T2**:
  New weights
* **__group_292__new_gradients** (optional) - **T3**:
  New gradients
* **__group_292__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_292__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_292__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_293__new_weights** (optional) - **T2**:
  New weights
* **__group_293__new_gradients** (optional) - **T3**:
  New gradients
* **__group_293__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_293__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_293__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_294__new_weights** (optional) - **T2**:
  New weights
* **__group_294__new_gradients** (optional) - **T3**:
  New gradients
* **__group_294__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_294__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_294__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_295__new_weights** (optional) - **T2**:
  New weights
* **__group_295__new_gradients** (optional) - **T3**:
  New gradients
* **__group_295__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_295__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_295__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_296__new_weights** (optional) - **T2**:
  New weights
* **__group_296__new_gradients** (optional) - **T3**:
  New gradients
* **__group_296__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_296__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_296__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_297__new_weights** (optional) - **T2**:
  New weights
* **__group_297__new_gradients** (optional) - **T3**:
  New gradients
* **__group_297__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_297__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_297__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_298__new_weights** (optional) - **T2**:
  New weights
* **__group_298__new_gradients** (optional) - **T3**:
  New gradients
* **__group_298__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_298__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_298__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_299__new_weights** (optional) - **T2**:
  New weights
* **__group_299__new_gradients** (optional) - **T3**:
  New gradients
* **__group_299__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_299__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_299__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_300__new_weights** (optional) - **T2**:
  New weights
* **__group_300__new_gradients** (optional) - **T3**:
  New gradients
* **__group_300__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_300__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_300__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_301__new_weights** (optional) - **T2**:
  New weights
* **__group_301__new_gradients** (optional) - **T3**:
  New gradients
* **__group_301__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_301__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_301__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_302__new_weights** (optional) - **T2**:
  New weights
* **__group_302__new_gradients** (optional) - **T3**:
  New gradients
* **__group_302__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_302__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_302__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_303__new_weights** (optional) - **T2**:
  New weights
* **__group_303__new_gradients** (optional) - **T3**:
  New gradients
* **__group_303__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_303__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_303__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_304__new_weights** (optional) - **T2**:
  New weights
* **__group_304__new_gradients** (optional) - **T3**:
  New gradients
* **__group_304__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_304__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_304__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_305__new_weights** (optional) - **T2**:
  New weights
* **__group_305__new_gradients** (optional) - **T3**:
  New gradients
* **__group_305__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_305__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_305__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_306__new_weights** (optional) - **T2**:
  New weights
* **__group_306__new_gradients** (optional) - **T3**:
  New gradients
* **__group_306__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_306__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_306__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_307__new_weights** (optional) - **T2**:
  New weights
* **__group_307__new_gradients** (optional) - **T3**:
  New gradients
* **__group_307__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_307__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_307__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_308__new_weights** (optional) - **T2**:
  New weights
* **__group_308__new_gradients** (optional) - **T3**:
  New gradients
* **__group_308__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_308__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_308__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_309__new_weights** (optional) - **T2**:
  New weights
* **__group_309__new_gradients** (optional) - **T3**:
  New gradients
* **__group_309__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_309__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_309__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_310__new_weights** (optional) - **T2**:
  New weights
* **__group_310__new_gradients** (optional) - **T3**:
  New gradients
* **__group_310__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_310__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_310__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_311__new_weights** (optional) - **T2**:
  New weights
* **__group_311__new_gradients** (optional) - **T3**:
  New gradients
* **__group_311__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_311__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_311__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_312__new_weights** (optional) - **T2**:
  New weights
* **__group_312__new_gradients** (optional) - **T3**:
  New gradients
* **__group_312__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_312__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_312__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_313__new_weights** (optional) - **T2**:
  New weights
* **__group_313__new_gradients** (optional) - **T3**:
  New gradients
* **__group_313__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_313__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_313__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_314__new_weights** (optional) - **T2**:
  New weights
* **__group_314__new_gradients** (optional) - **T3**:
  New gradients
* **__group_314__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_314__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_314__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_315__new_weights** (optional) - **T2**:
  New weights
* **__group_315__new_gradients** (optional) - **T3**:
  New gradients
* **__group_315__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_315__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_315__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_316__new_weights** (optional) - **T2**:
  New weights
* **__group_316__new_gradients** (optional) - **T3**:
  New gradients
* **__group_316__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_316__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_316__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_317__new_weights** (optional) - **T2**:
  New weights
* **__group_317__new_gradients** (optional) - **T3**:
  New gradients
* **__group_317__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_317__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_317__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_318__new_weights** (optional) - **T2**:
  New weights
* **__group_318__new_gradients** (optional) - **T3**:
  New gradients
* **__group_318__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_318__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_318__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_319__new_weights** (optional) - **T2**:
  New weights
* **__group_319__new_gradients** (optional) - **T3**:
  New gradients
* **__group_319__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_319__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_319__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_320__new_weights** (optional) - **T2**:
  New weights
* **__group_320__new_gradients** (optional) - **T3**:
  New gradients
* **__group_320__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_320__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_320__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_321__new_weights** (optional) - **T2**:
  New weights
* **__group_321__new_gradients** (optional) - **T3**:
  New gradients
* **__group_321__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_321__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_321__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_322__new_weights** (optional) - **T2**:
  New weights
* **__group_322__new_gradients** (optional) - **T3**:
  New gradients
* **__group_322__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_322__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_322__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_323__new_weights** (optional) - **T2**:
  New weights
* **__group_323__new_gradients** (optional) - **T3**:
  New gradients
* **__group_323__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_323__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_323__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_324__new_weights** (optional) - **T2**:
  New weights
* **__group_324__new_gradients** (optional) - **T3**:
  New gradients
* **__group_324__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_324__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_324__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_325__new_weights** (optional) - **T2**:
  New weights
* **__group_325__new_gradients** (optional) - **T3**:
  New gradients
* **__group_325__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_325__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_325__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_326__new_weights** (optional) - **T2**:
  New weights
* **__group_326__new_gradients** (optional) - **T3**:
  New gradients
* **__group_326__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_326__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_326__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_327__new_weights** (optional) - **T2**:
  New weights
* **__group_327__new_gradients** (optional) - **T3**:
  New gradients
* **__group_327__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_327__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_327__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_328__new_weights** (optional) - **T2**:
  New weights
* **__group_328__new_gradients** (optional) - **T3**:
  New gradients
* **__group_328__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_328__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_328__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_329__new_weights** (optional) - **T2**:
  New weights
* **__group_329__new_gradients** (optional) - **T3**:
  New gradients
* **__group_329__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_329__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_329__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_330__new_weights** (optional) - **T2**:
  New weights
* **__group_330__new_gradients** (optional) - **T3**:
  New gradients
* **__group_330__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_330__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_330__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_331__new_weights** (optional) - **T2**:
  New weights
* **__group_331__new_gradients** (optional) - **T3**:
  New gradients
* **__group_331__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_331__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_331__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_332__new_weights** (optional) - **T2**:
  New weights
* **__group_332__new_gradients** (optional) - **T3**:
  New gradients
* **__group_332__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_332__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_332__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_333__new_weights** (optional) - **T2**:
  New weights
* **__group_333__new_gradients** (optional) - **T3**:
  New gradients
* **__group_333__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_333__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_333__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_334__new_weights** (optional) - **T2**:
  New weights
* **__group_334__new_gradients** (optional) - **T3**:
  New gradients
* **__group_334__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_334__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_334__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_335__new_weights** (optional) - **T2**:
  New weights
* **__group_335__new_gradients** (optional) - **T3**:
  New gradients
* **__group_335__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_335__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_335__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_336__new_weights** (optional) - **T2**:
  New weights
* **__group_336__new_gradients** (optional) - **T3**:
  New gradients
* **__group_336__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_336__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_336__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_337__new_weights** (optional) - **T2**:
  New weights
* **__group_337__new_gradients** (optional) - **T3**:
  New gradients
* **__group_337__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_337__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_337__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_338__new_weights** (optional) - **T2**:
  New weights
* **__group_338__new_gradients** (optional) - **T3**:
  New gradients
* **__group_338__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_338__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_338__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_339__new_weights** (optional) - **T2**:
  New weights
* **__group_339__new_gradients** (optional) - **T3**:
  New gradients
* **__group_339__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_339__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_339__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_340__new_weights** (optional) - **T2**:
  New weights
* **__group_340__new_gradients** (optional) - **T3**:
  New gradients
* **__group_340__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_340__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_340__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_341__new_weights** (optional) - **T2**:
  New weights
* **__group_341__new_gradients** (optional) - **T3**:
  New gradients
* **__group_341__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_341__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_341__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_342__new_weights** (optional) - **T2**:
  New weights
* **__group_342__new_gradients** (optional) - **T3**:
  New gradients
* **__group_342__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_342__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_342__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_343__new_weights** (optional) - **T2**:
  New weights
* **__group_343__new_gradients** (optional) - **T3**:
  New gradients
* **__group_343__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_343__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_343__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_344__new_weights** (optional) - **T2**:
  New weights
* **__group_344__new_gradients** (optional) - **T3**:
  New gradients
* **__group_344__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_344__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_344__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_345__new_weights** (optional) - **T2**:
  New weights
* **__group_345__new_gradients** (optional) - **T3**:
  New gradients
* **__group_345__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_345__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_345__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_346__new_weights** (optional) - **T2**:
  New weights
* **__group_346__new_gradients** (optional) - **T3**:
  New gradients
* **__group_346__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_346__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_346__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_347__new_weights** (optional) - **T2**:
  New weights
* **__group_347__new_gradients** (optional) - **T3**:
  New gradients
* **__group_347__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_347__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_347__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_348__new_weights** (optional) - **T2**:
  New weights
* **__group_348__new_gradients** (optional) - **T3**:
  New gradients
* **__group_348__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_348__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_348__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_349__new_weights** (optional) - **T2**:
  New weights
* **__group_349__new_gradients** (optional) - **T3**:
  New gradients
* **__group_349__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_349__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_349__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_350__new_weights** (optional) - **T2**:
  New weights
* **__group_350__new_gradients** (optional) - **T3**:
  New gradients
* **__group_350__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_350__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_350__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_351__new_weights** (optional) - **T2**:
  New weights
* **__group_351__new_gradients** (optional) - **T3**:
  New gradients
* **__group_351__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_351__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_351__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_352__new_weights** (optional) - **T2**:
  New weights
* **__group_352__new_gradients** (optional) - **T3**:
  New gradients
* **__group_352__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_352__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_352__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_353__new_weights** (optional) - **T2**:
  New weights
* **__group_353__new_gradients** (optional) - **T3**:
  New gradients
* **__group_353__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_353__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_353__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_354__new_weights** (optional) - **T2**:
  New weights
* **__group_354__new_gradients** (optional) - **T3**:
  New gradients
* **__group_354__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_354__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_354__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_355__new_weights** (optional) - **T2**:
  New weights
* **__group_355__new_gradients** (optional) - **T3**:
  New gradients
* **__group_355__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_355__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_355__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_356__new_weights** (optional) - **T2**:
  New weights
* **__group_356__new_gradients** (optional) - **T3**:
  New gradients
* **__group_356__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_356__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_356__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_357__new_weights** (optional) - **T2**:
  New weights
* **__group_357__new_gradients** (optional) - **T3**:
  New gradients
* **__group_357__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_357__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_357__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_358__new_weights** (optional) - **T2**:
  New weights
* **__group_358__new_gradients** (optional) - **T3**:
  New gradients
* **__group_358__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_358__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_358__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_359__new_weights** (optional) - **T2**:
  New weights
* **__group_359__new_gradients** (optional) - **T3**:
  New gradients
* **__group_359__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_359__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_359__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_360__new_weights** (optional) - **T2**:
  New weights
* **__group_360__new_gradients** (optional) - **T3**:
  New gradients
* **__group_360__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_360__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_360__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_361__new_weights** (optional) - **T2**:
  New weights
* **__group_361__new_gradients** (optional) - **T3**:
  New gradients
* **__group_361__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_361__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_361__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_362__new_weights** (optional) - **T2**:
  New weights
* **__group_362__new_gradients** (optional) - **T3**:
  New gradients
* **__group_362__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_362__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_362__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_363__new_weights** (optional) - **T2**:
  New weights
* **__group_363__new_gradients** (optional) - **T3**:
  New gradients
* **__group_363__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_363__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_363__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_364__new_weights** (optional) - **T2**:
  New weights
* **__group_364__new_gradients** (optional) - **T3**:
  New gradients
* **__group_364__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_364__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_364__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_365__new_weights** (optional) - **T2**:
  New weights
* **__group_365__new_gradients** (optional) - **T3**:
  New gradients
* **__group_365__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_365__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_365__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_366__new_weights** (optional) - **T2**:
  New weights
* **__group_366__new_gradients** (optional) - **T3**:
  New gradients
* **__group_366__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_366__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_366__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_367__new_weights** (optional) - **T2**:
  New weights
* **__group_367__new_gradients** (optional) - **T3**:
  New gradients
* **__group_367__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_367__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_367__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_368__new_weights** (optional) - **T2**:
  New weights
* **__group_368__new_gradients** (optional) - **T3**:
  New gradients
* **__group_368__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_368__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_368__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_369__new_weights** (optional) - **T2**:
  New weights
* **__group_369__new_gradients** (optional) - **T3**:
  New gradients
* **__group_369__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_369__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_369__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_370__new_weights** (optional) - **T2**:
  New weights
* **__group_370__new_gradients** (optional) - **T3**:
  New gradients
* **__group_370__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_370__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_370__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_371__new_weights** (optional) - **T2**:
  New weights
* **__group_371__new_gradients** (optional) - **T3**:
  New gradients
* **__group_371__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_371__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_371__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_372__new_weights** (optional) - **T2**:
  New weights
* **__group_372__new_gradients** (optional) - **T3**:
  New gradients
* **__group_372__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_372__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_372__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_373__new_weights** (optional) - **T2**:
  New weights
* **__group_373__new_gradients** (optional) - **T3**:
  New gradients
* **__group_373__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_373__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_373__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_374__new_weights** (optional) - **T2**:
  New weights
* **__group_374__new_gradients** (optional) - **T3**:
  New gradients
* **__group_374__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_374__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_374__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_375__new_weights** (optional) - **T2**:
  New weights
* **__group_375__new_gradients** (optional) - **T3**:
  New gradients
* **__group_375__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_375__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_375__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_376__new_weights** (optional) - **T2**:
  New weights
* **__group_376__new_gradients** (optional) - **T3**:
  New gradients
* **__group_376__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_376__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_376__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_377__new_weights** (optional) - **T2**:
  New weights
* **__group_377__new_gradients** (optional) - **T3**:
  New gradients
* **__group_377__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_377__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_377__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_378__new_weights** (optional) - **T2**:
  New weights
* **__group_378__new_gradients** (optional) - **T3**:
  New gradients
* **__group_378__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_378__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_378__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_379__new_weights** (optional) - **T2**:
  New weights
* **__group_379__new_gradients** (optional) - **T3**:
  New gradients
* **__group_379__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_379__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_379__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_380__new_weights** (optional) - **T2**:
  New weights
* **__group_380__new_gradients** (optional) - **T3**:
  New gradients
* **__group_380__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_380__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_380__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_381__new_weights** (optional) - **T2**:
  New weights
* **__group_381__new_gradients** (optional) - **T3**:
  New gradients
* **__group_381__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_381__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_381__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_382__new_weights** (optional) - **T2**:
  New weights
* **__group_382__new_gradients** (optional) - **T3**:
  New gradients
* **__group_382__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_382__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_382__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_383__new_weights** (optional) - **T2**:
  New weights
* **__group_383__new_gradients** (optional) - **T3**:
  New gradients
* **__group_383__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_383__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_383__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_384__new_weights** (optional) - **T2**:
  New weights
* **__group_384__new_gradients** (optional) - **T3**:
  New gradients
* **__group_384__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_384__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_384__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_385__new_weights** (optional) - **T2**:
  New weights
* **__group_385__new_gradients** (optional) - **T3**:
  New gradients
* **__group_385__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_385__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_385__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_386__new_weights** (optional) - **T2**:
  New weights
* **__group_386__new_gradients** (optional) - **T3**:
  New gradients
* **__group_386__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_386__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_386__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_387__new_weights** (optional) - **T2**:
  New weights
* **__group_387__new_gradients** (optional) - **T3**:
  New gradients
* **__group_387__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_387__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_387__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_388__new_weights** (optional) - **T2**:
  New weights
* **__group_388__new_gradients** (optional) - **T3**:
  New gradients
* **__group_388__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_388__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_388__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_389__new_weights** (optional) - **T2**:
  New weights
* **__group_389__new_gradients** (optional) - **T3**:
  New gradients
* **__group_389__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_389__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_389__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_390__new_weights** (optional) - **T2**:
  New weights
* **__group_390__new_gradients** (optional) - **T3**:
  New gradients
* **__group_390__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_390__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_390__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_391__new_weights** (optional) - **T2**:
  New weights
* **__group_391__new_gradients** (optional) - **T3**:
  New gradients
* **__group_391__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_391__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_391__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_392__new_weights** (optional) - **T2**:
  New weights
* **__group_392__new_gradients** (optional) - **T3**:
  New gradients
* **__group_392__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_392__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_392__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_393__new_weights** (optional) - **T2**:
  New weights
* **__group_393__new_gradients** (optional) - **T3**:
  New gradients
* **__group_393__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_393__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_393__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_394__new_weights** (optional) - **T2**:
  New weights
* **__group_394__new_gradients** (optional) - **T3**:
  New gradients
* **__group_394__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_394__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_394__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_395__new_weights** (optional) - **T2**:
  New weights
* **__group_395__new_gradients** (optional) - **T3**:
  New gradients
* **__group_395__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_395__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_395__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_396__new_weights** (optional) - **T2**:
  New weights
* **__group_396__new_gradients** (optional) - **T3**:
  New gradients
* **__group_396__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_396__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_396__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_397__new_weights** (optional) - **T2**:
  New weights
* **__group_397__new_gradients** (optional) - **T3**:
  New gradients
* **__group_397__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_397__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_397__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_398__new_weights** (optional) - **T2**:
  New weights
* **__group_398__new_gradients** (optional) - **T3**:
  New gradients
* **__group_398__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_398__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_398__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_399__new_weights** (optional) - **T2**:
  New weights
* **__group_399__new_gradients** (optional) - **T3**:
  New gradients
* **__group_399__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_399__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_399__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_400__new_weights** (optional) - **T2**:
  New weights
* **__group_400__new_gradients** (optional) - **T3**:
  New gradients
* **__group_400__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_400__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_400__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_401__new_weights** (optional) - **T2**:
  New weights
* **__group_401__new_gradients** (optional) - **T3**:
  New gradients
* **__group_401__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_401__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_401__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_402__new_weights** (optional) - **T2**:
  New weights
* **__group_402__new_gradients** (optional) - **T3**:
  New gradients
* **__group_402__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_402__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_402__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_403__new_weights** (optional) - **T2**:
  New weights
* **__group_403__new_gradients** (optional) - **T3**:
  New gradients
* **__group_403__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_403__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_403__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_404__new_weights** (optional) - **T2**:
  New weights
* **__group_404__new_gradients** (optional) - **T3**:
  New gradients
* **__group_404__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_404__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_404__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_405__new_weights** (optional) - **T2**:
  New weights
* **__group_405__new_gradients** (optional) - **T3**:
  New gradients
* **__group_405__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_405__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_405__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_406__new_weights** (optional) - **T2**:
  New weights
* **__group_406__new_gradients** (optional) - **T3**:
  New gradients
* **__group_406__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_406__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_406__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_407__new_weights** (optional) - **T2**:
  New weights
* **__group_407__new_gradients** (optional) - **T3**:
  New gradients
* **__group_407__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_407__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_407__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_408__new_weights** (optional) - **T2**:
  New weights
* **__group_408__new_gradients** (optional) - **T3**:
  New gradients
* **__group_408__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_408__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_408__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_409__new_weights** (optional) - **T2**:
  New weights
* **__group_409__new_gradients** (optional) - **T3**:
  New gradients
* **__group_409__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_409__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_409__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_410__new_weights** (optional) - **T2**:
  New weights
* **__group_410__new_gradients** (optional) - **T3**:
  New gradients
* **__group_410__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_410__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_410__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_411__new_weights** (optional) - **T2**:
  New weights
* **__group_411__new_gradients** (optional) - **T3**:
  New gradients
* **__group_411__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_411__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_411__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_412__new_weights** (optional) - **T2**:
  New weights
* **__group_412__new_gradients** (optional) - **T3**:
  New gradients
* **__group_412__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_412__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_412__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_413__new_weights** (optional) - **T2**:
  New weights
* **__group_413__new_gradients** (optional) - **T3**:
  New gradients
* **__group_413__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_413__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_413__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_414__new_weights** (optional) - **T2**:
  New weights
* **__group_414__new_gradients** (optional) - **T3**:
  New gradients
* **__group_414__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_414__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_414__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_415__new_weights** (optional) - **T2**:
  New weights
* **__group_415__new_gradients** (optional) - **T3**:
  New gradients
* **__group_415__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_415__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_415__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_416__new_weights** (optional) - **T2**:
  New weights
* **__group_416__new_gradients** (optional) - **T3**:
  New gradients
* **__group_416__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_416__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_416__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_417__new_weights** (optional) - **T2**:
  New weights
* **__group_417__new_gradients** (optional) - **T3**:
  New gradients
* **__group_417__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_417__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_417__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_418__new_weights** (optional) - **T2**:
  New weights
* **__group_418__new_gradients** (optional) - **T3**:
  New gradients
* **__group_418__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_418__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_418__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_419__new_weights** (optional) - **T2**:
  New weights
* **__group_419__new_gradients** (optional) - **T3**:
  New gradients
* **__group_419__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_419__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_419__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_420__new_weights** (optional) - **T2**:
  New weights
* **__group_420__new_gradients** (optional) - **T3**:
  New gradients
* **__group_420__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_420__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_420__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_421__new_weights** (optional) - **T2**:
  New weights
* **__group_421__new_gradients** (optional) - **T3**:
  New gradients
* **__group_421__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_421__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_421__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_422__new_weights** (optional) - **T2**:
  New weights
* **__group_422__new_gradients** (optional) - **T3**:
  New gradients
* **__group_422__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_422__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_422__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_423__new_weights** (optional) - **T2**:
  New weights
* **__group_423__new_gradients** (optional) - **T3**:
  New gradients
* **__group_423__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_423__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_423__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_424__new_weights** (optional) - **T2**:
  New weights
* **__group_424__new_gradients** (optional) - **T3**:
  New gradients
* **__group_424__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_424__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_424__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_425__new_weights** (optional) - **T2**:
  New weights
* **__group_425__new_gradients** (optional) - **T3**:
  New gradients
* **__group_425__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_425__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_425__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_426__new_weights** (optional) - **T2**:
  New weights
* **__group_426__new_gradients** (optional) - **T3**:
  New gradients
* **__group_426__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_426__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_426__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_427__new_weights** (optional) - **T2**:
  New weights
* **__group_427__new_gradients** (optional) - **T3**:
  New gradients
* **__group_427__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_427__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_427__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_428__new_weights** (optional) - **T2**:
  New weights
* **__group_428__new_gradients** (optional) - **T3**:
  New gradients
* **__group_428__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_428__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_428__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_429__new_weights** (optional) - **T2**:
  New weights
* **__group_429__new_gradients** (optional) - **T3**:
  New gradients
* **__group_429__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_429__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_429__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_430__new_weights** (optional) - **T2**:
  New weights
* **__group_430__new_gradients** (optional) - **T3**:
  New gradients
* **__group_430__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_430__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_430__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_431__new_weights** (optional) - **T2**:
  New weights
* **__group_431__new_gradients** (optional) - **T3**:
  New gradients
* **__group_431__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_431__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_431__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_432__new_weights** (optional) - **T2**:
  New weights
* **__group_432__new_gradients** (optional) - **T3**:
  New gradients
* **__group_432__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_432__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_432__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_433__new_weights** (optional) - **T2**:
  New weights
* **__group_433__new_gradients** (optional) - **T3**:
  New gradients
* **__group_433__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_433__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_433__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_434__new_weights** (optional) - **T2**:
  New weights
* **__group_434__new_gradients** (optional) - **T3**:
  New gradients
* **__group_434__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_434__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_434__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_435__new_weights** (optional) - **T2**:
  New weights
* **__group_435__new_gradients** (optional) - **T3**:
  New gradients
* **__group_435__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_435__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_435__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_436__new_weights** (optional) - **T2**:
  New weights
* **__group_436__new_gradients** (optional) - **T3**:
  New gradients
* **__group_436__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_436__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_436__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_437__new_weights** (optional) - **T2**:
  New weights
* **__group_437__new_gradients** (optional) - **T3**:
  New gradients
* **__group_437__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_437__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_437__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_438__new_weights** (optional) - **T2**:
  New weights
* **__group_438__new_gradients** (optional) - **T3**:
  New gradients
* **__group_438__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_438__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_438__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_439__new_weights** (optional) - **T2**:
  New weights
* **__group_439__new_gradients** (optional) - **T3**:
  New gradients
* **__group_439__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_439__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_439__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_440__new_weights** (optional) - **T2**:
  New weights
* **__group_440__new_gradients** (optional) - **T3**:
  New gradients
* **__group_440__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_440__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_440__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_441__new_weights** (optional) - **T2**:
  New weights
* **__group_441__new_gradients** (optional) - **T3**:
  New gradients
* **__group_441__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_441__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_441__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_442__new_weights** (optional) - **T2**:
  New weights
* **__group_442__new_gradients** (optional) - **T3**:
  New gradients
* **__group_442__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_442__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_442__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_443__new_weights** (optional) - **T2**:
  New weights
* **__group_443__new_gradients** (optional) - **T3**:
  New gradients
* **__group_443__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_443__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_443__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_444__new_weights** (optional) - **T2**:
  New weights
* **__group_444__new_gradients** (optional) - **T3**:
  New gradients
* **__group_444__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_444__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_444__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_445__new_weights** (optional) - **T2**:
  New weights
* **__group_445__new_gradients** (optional) - **T3**:
  New gradients
* **__group_445__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_445__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_445__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_446__new_weights** (optional) - **T2**:
  New weights
* **__group_446__new_gradients** (optional) - **T3**:
  New gradients
* **__group_446__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_446__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_446__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_447__new_weights** (optional) - **T2**:
  New weights
* **__group_447__new_gradients** (optional) - **T3**:
  New gradients
* **__group_447__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_447__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_447__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_448__new_weights** (optional) - **T2**:
  New weights
* **__group_448__new_gradients** (optional) - **T3**:
  New gradients
* **__group_448__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_448__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_448__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_449__new_weights** (optional) - **T2**:
  New weights
* **__group_449__new_gradients** (optional) - **T3**:
  New gradients
* **__group_449__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_449__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_449__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_450__new_weights** (optional) - **T2**:
  New weights
* **__group_450__new_gradients** (optional) - **T3**:
  New gradients
* **__group_450__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_450__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_450__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_451__new_weights** (optional) - **T2**:
  New weights
* **__group_451__new_gradients** (optional) - **T3**:
  New gradients
* **__group_451__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_451__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_451__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_452__new_weights** (optional) - **T2**:
  New weights
* **__group_452__new_gradients** (optional) - **T3**:
  New gradients
* **__group_452__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_452__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_452__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_453__new_weights** (optional) - **T2**:
  New weights
* **__group_453__new_gradients** (optional) - **T3**:
  New gradients
* **__group_453__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_453__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_453__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_454__new_weights** (optional) - **T2**:
  New weights
* **__group_454__new_gradients** (optional) - **T3**:
  New gradients
* **__group_454__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_454__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_454__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_455__new_weights** (optional) - **T2**:
  New weights
* **__group_455__new_gradients** (optional) - **T3**:
  New gradients
* **__group_455__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_455__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_455__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_456__new_weights** (optional) - **T2**:
  New weights
* **__group_456__new_gradients** (optional) - **T3**:
  New gradients
* **__group_456__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_456__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_456__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_457__new_weights** (optional) - **T2**:
  New weights
* **__group_457__new_gradients** (optional) - **T3**:
  New gradients
* **__group_457__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_457__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_457__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_458__new_weights** (optional) - **T2**:
  New weights
* **__group_458__new_gradients** (optional) - **T3**:
  New gradients
* **__group_458__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_458__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_458__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_459__new_weights** (optional) - **T2**:
  New weights
* **__group_459__new_gradients** (optional) - **T3**:
  New gradients
* **__group_459__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_459__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_459__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_460__new_weights** (optional) - **T2**:
  New weights
* **__group_460__new_gradients** (optional) - **T3**:
  New gradients
* **__group_460__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_460__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_460__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_461__new_weights** (optional) - **T2**:
  New weights
* **__group_461__new_gradients** (optional) - **T3**:
  New gradients
* **__group_461__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_461__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_461__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_462__new_weights** (optional) - **T2**:
  New weights
* **__group_462__new_gradients** (optional) - **T3**:
  New gradients
* **__group_462__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_462__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_462__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_463__new_weights** (optional) - **T2**:
  New weights
* **__group_463__new_gradients** (optional) - **T3**:
  New gradients
* **__group_463__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_463__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_463__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_464__new_weights** (optional) - **T2**:
  New weights
* **__group_464__new_gradients** (optional) - **T3**:
  New gradients
* **__group_464__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_464__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_464__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_465__new_weights** (optional) - **T2**:
  New weights
* **__group_465__new_gradients** (optional) - **T3**:
  New gradients
* **__group_465__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_465__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_465__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_466__new_weights** (optional) - **T2**:
  New weights
* **__group_466__new_gradients** (optional) - **T3**:
  New gradients
* **__group_466__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_466__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_466__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_467__new_weights** (optional) - **T2**:
  New weights
* **__group_467__new_gradients** (optional) - **T3**:
  New gradients
* **__group_467__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_467__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_467__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_468__new_weights** (optional) - **T2**:
  New weights
* **__group_468__new_gradients** (optional) - **T3**:
  New gradients
* **__group_468__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_468__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_468__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_469__new_weights** (optional) - **T2**:
  New weights
* **__group_469__new_gradients** (optional) - **T3**:
  New gradients
* **__group_469__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_469__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_469__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_470__new_weights** (optional) - **T2**:
  New weights
* **__group_470__new_gradients** (optional) - **T3**:
  New gradients
* **__group_470__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_470__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_470__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_471__new_weights** (optional) - **T2**:
  New weights
* **__group_471__new_gradients** (optional) - **T3**:
  New gradients
* **__group_471__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_471__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_471__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_472__new_weights** (optional) - **T2**:
  New weights
* **__group_472__new_gradients** (optional) - **T3**:
  New gradients
* **__group_472__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_472__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_472__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_473__new_weights** (optional) - **T2**:
  New weights
* **__group_473__new_gradients** (optional) - **T3**:
  New gradients
* **__group_473__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_473__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_473__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_474__new_weights** (optional) - **T2**:
  New weights
* **__group_474__new_gradients** (optional) - **T3**:
  New gradients
* **__group_474__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_474__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_474__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_475__new_weights** (optional) - **T2**:
  New weights
* **__group_475__new_gradients** (optional) - **T3**:
  New gradients
* **__group_475__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_475__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_475__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_476__new_weights** (optional) - **T2**:
  New weights
* **__group_476__new_gradients** (optional) - **T3**:
  New gradients
* **__group_476__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_476__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_476__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_477__new_weights** (optional) - **T2**:
  New weights
* **__group_477__new_gradients** (optional) - **T3**:
  New gradients
* **__group_477__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_477__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_477__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_478__new_weights** (optional) - **T2**:
  New weights
* **__group_478__new_gradients** (optional) - **T3**:
  New gradients
* **__group_478__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_478__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_478__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_479__new_weights** (optional) - **T2**:
  New weights
* **__group_479__new_gradients** (optional) - **T3**:
  New gradients
* **__group_479__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_479__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_479__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_480__new_weights** (optional) - **T2**:
  New weights
* **__group_480__new_gradients** (optional) - **T3**:
  New gradients
* **__group_480__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_480__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_480__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_481__new_weights** (optional) - **T2**:
  New weights
* **__group_481__new_gradients** (optional) - **T3**:
  New gradients
* **__group_481__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_481__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_481__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_482__new_weights** (optional) - **T2**:
  New weights
* **__group_482__new_gradients** (optional) - **T3**:
  New gradients
* **__group_482__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_482__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_482__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_483__new_weights** (optional) - **T2**:
  New weights
* **__group_483__new_gradients** (optional) - **T3**:
  New gradients
* **__group_483__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_483__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_483__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_484__new_weights** (optional) - **T2**:
  New weights
* **__group_484__new_gradients** (optional) - **T3**:
  New gradients
* **__group_484__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_484__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_484__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_485__new_weights** (optional) - **T2**:
  New weights
* **__group_485__new_gradients** (optional) - **T3**:
  New gradients
* **__group_485__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_485__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_485__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_486__new_weights** (optional) - **T2**:
  New weights
* **__group_486__new_gradients** (optional) - **T3**:
  New gradients
* **__group_486__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_486__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_486__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_487__new_weights** (optional) - **T2**:
  New weights
* **__group_487__new_gradients** (optional) - **T3**:
  New gradients
* **__group_487__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_487__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_487__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_488__new_weights** (optional) - **T2**:
  New weights
* **__group_488__new_gradients** (optional) - **T3**:
  New gradients
* **__group_488__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_488__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_488__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_489__new_weights** (optional) - **T2**:
  New weights
* **__group_489__new_gradients** (optional) - **T3**:
  New gradients
* **__group_489__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_489__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_489__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_490__new_weights** (optional) - **T2**:
  New weights
* **__group_490__new_gradients** (optional) - **T3**:
  New gradients
* **__group_490__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_490__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_490__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_491__new_weights** (optional) - **T2**:
  New weights
* **__group_491__new_gradients** (optional) - **T3**:
  New gradients
* **__group_491__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_491__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_491__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_492__new_weights** (optional) - **T2**:
  New weights
* **__group_492__new_gradients** (optional) - **T3**:
  New gradients
* **__group_492__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_492__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_492__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_493__new_weights** (optional) - **T2**:
  New weights
* **__group_493__new_gradients** (optional) - **T3**:
  New gradients
* **__group_493__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_493__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_493__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_494__new_weights** (optional) - **T2**:
  New weights
* **__group_494__new_gradients** (optional) - **T3**:
  New gradients
* **__group_494__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_494__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_494__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_495__new_weights** (optional) - **T2**:
  New weights
* **__group_495__new_gradients** (optional) - **T3**:
  New gradients
* **__group_495__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_495__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_495__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_496__new_weights** (optional) - **T2**:
  New weights
* **__group_496__new_gradients** (optional) - **T3**:
  New gradients
* **__group_496__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_496__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_496__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_497__new_weights** (optional) - **T2**:
  New weights
* **__group_497__new_gradients** (optional) - **T3**:
  New gradients
* **__group_497__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_497__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_497__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_498__new_weights** (optional) - **T2**:
  New weights
* **__group_498__new_gradients** (optional) - **T3**:
  New gradients
* **__group_498__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_498__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_498__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_499__new_weights** (optional) - **T2**:
  New weights
* **__group_499__new_gradients** (optional) - **T3**:
  New gradients
* **__group_499__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_499__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_499__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_500__new_weights** (optional) - **T2**:
  New weights
* **__group_500__new_gradients** (optional) - **T3**:
  New gradients
* **__group_500__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_500__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_500__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_501__new_weights** (optional) - **T2**:
  New weights
* **__group_501__new_gradients** (optional) - **T3**:
  New gradients
* **__group_501__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_501__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_501__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_502__new_weights** (optional) - **T2**:
  New weights
* **__group_502__new_gradients** (optional) - **T3**:
  New gradients
* **__group_502__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_502__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_502__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_503__new_weights** (optional) - **T2**:
  New weights
* **__group_503__new_gradients** (optional) - **T3**:
  New gradients
* **__group_503__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_503__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_503__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_504__new_weights** (optional) - **T2**:
  New weights
* **__group_504__new_gradients** (optional) - **T3**:
  New gradients
* **__group_504__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_504__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_504__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_505__new_weights** (optional) - **T2**:
  New weights
* **__group_505__new_gradients** (optional) - **T3**:
  New gradients
* **__group_505__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_505__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_505__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_506__new_weights** (optional) - **T2**:
  New weights
* **__group_506__new_gradients** (optional) - **T3**:
  New gradients
* **__group_506__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_506__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_506__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_507__new_weights** (optional) - **T2**:
  New weights
* **__group_507__new_gradients** (optional) - **T3**:
  New gradients
* **__group_507__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_507__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_507__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_508__new_weights** (optional) - **T2**:
  New weights
* **__group_508__new_gradients** (optional) - **T3**:
  New gradients
* **__group_508__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_508__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_508__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_509__new_weights** (optional) - **T2**:
  New weights
* **__group_509__new_gradients** (optional) - **T3**:
  New gradients
* **__group_509__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_509__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_509__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_510__new_weights** (optional) - **T2**:
  New weights
* **__group_510__new_gradients** (optional) - **T3**:
  New gradients
* **__group_510__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_510__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_510__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_511__new_weights** (optional) - **T2**:
  New weights
* **__group_511__new_gradients** (optional) - **T3**:
  New gradients
* **__group_511__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_511__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_511__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_512__new_weights** (optional) - **T2**:
  New weights
* **__group_512__new_gradients** (optional) - **T3**:
  New gradients
* **__group_512__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_512__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_512__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_513__new_weights** (optional) - **T2**:
  New weights
* **__group_513__new_gradients** (optional) - **T3**:
  New gradients
* **__group_513__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_513__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_513__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_514__new_weights** (optional) - **T2**:
  New weights
* **__group_514__new_gradients** (optional) - **T3**:
  New gradients
* **__group_514__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_514__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_514__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_515__new_weights** (optional) - **T2**:
  New weights
* **__group_515__new_gradients** (optional) - **T3**:
  New gradients
* **__group_515__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_515__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_515__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_516__new_weights** (optional) - **T2**:
  New weights
* **__group_516__new_gradients** (optional) - **T3**:
  New gradients
* **__group_516__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_516__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_516__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_517__new_weights** (optional) - **T2**:
  New weights
* **__group_517__new_gradients** (optional) - **T3**:
  New gradients
* **__group_517__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_517__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_517__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_518__new_weights** (optional) - **T2**:
  New weights
* **__group_518__new_gradients** (optional) - **T3**:
  New gradients
* **__group_518__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_518__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_518__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_519__new_weights** (optional) - **T2**:
  New weights
* **__group_519__new_gradients** (optional) - **T3**:
  New gradients
* **__group_519__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_519__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_519__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_520__new_weights** (optional) - **T2**:
  New weights
* **__group_520__new_gradients** (optional) - **T3**:
  New gradients
* **__group_520__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_520__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_520__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_521__new_weights** (optional) - **T2**:
  New weights
* **__group_521__new_gradients** (optional) - **T3**:
  New gradients
* **__group_521__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_521__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_521__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_522__new_weights** (optional) - **T2**:
  New weights
* **__group_522__new_gradients** (optional) - **T3**:
  New gradients
* **__group_522__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_522__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_522__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_523__new_weights** (optional) - **T2**:
  New weights
* **__group_523__new_gradients** (optional) - **T3**:
  New gradients
* **__group_523__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_523__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_523__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_524__new_weights** (optional) - **T2**:
  New weights
* **__group_524__new_gradients** (optional) - **T3**:
  New gradients
* **__group_524__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_524__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_524__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_525__new_weights** (optional) - **T2**:
  New weights
* **__group_525__new_gradients** (optional) - **T3**:
  New gradients
* **__group_525__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_525__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_525__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_526__new_weights** (optional) - **T2**:
  New weights
* **__group_526__new_gradients** (optional) - **T3**:
  New gradients
* **__group_526__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_526__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_526__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_527__new_weights** (optional) - **T2**:
  New weights
* **__group_527__new_gradients** (optional) - **T3**:
  New gradients
* **__group_527__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_527__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_527__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_528__new_weights** (optional) - **T2**:
  New weights
* **__group_528__new_gradients** (optional) - **T3**:
  New gradients
* **__group_528__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_528__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_528__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_529__new_weights** (optional) - **T2**:
  New weights
* **__group_529__new_gradients** (optional) - **T3**:
  New gradients
* **__group_529__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_529__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_529__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_530__new_weights** (optional) - **T2**:
  New weights
* **__group_530__new_gradients** (optional) - **T3**:
  New gradients
* **__group_530__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_530__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_530__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_531__new_weights** (optional) - **T2**:
  New weights
* **__group_531__new_gradients** (optional) - **T3**:
  New gradients
* **__group_531__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_531__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_531__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_532__new_weights** (optional) - **T2**:
  New weights
* **__group_532__new_gradients** (optional) - **T3**:
  New gradients
* **__group_532__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_532__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_532__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_533__new_weights** (optional) - **T2**:
  New weights
* **__group_533__new_gradients** (optional) - **T3**:
  New gradients
* **__group_533__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_533__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_533__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_534__new_weights** (optional) - **T2**:
  New weights
* **__group_534__new_gradients** (optional) - **T3**:
  New gradients
* **__group_534__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_534__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_534__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_535__new_weights** (optional) - **T2**:
  New weights
* **__group_535__new_gradients** (optional) - **T3**:
  New gradients
* **__group_535__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_535__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_535__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_536__new_weights** (optional) - **T2**:
  New weights
* **__group_536__new_gradients** (optional) - **T3**:
  New gradients
* **__group_536__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_536__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_536__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_537__new_weights** (optional) - **T2**:
  New weights
* **__group_537__new_gradients** (optional) - **T3**:
  New gradients
* **__group_537__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_537__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_537__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_538__new_weights** (optional) - **T2**:
  New weights
* **__group_538__new_gradients** (optional) - **T3**:
  New gradients
* **__group_538__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_538__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_538__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_539__new_weights** (optional) - **T2**:
  New weights
* **__group_539__new_gradients** (optional) - **T3**:
  New gradients
* **__group_539__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_539__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_539__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_540__new_weights** (optional) - **T2**:
  New weights
* **__group_540__new_gradients** (optional) - **T3**:
  New gradients
* **__group_540__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_540__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_540__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_541__new_weights** (optional) - **T2**:
  New weights
* **__group_541__new_gradients** (optional) - **T3**:
  New gradients
* **__group_541__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_541__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_541__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_542__new_weights** (optional) - **T2**:
  New weights
* **__group_542__new_gradients** (optional) - **T3**:
  New gradients
* **__group_542__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_542__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_542__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_543__new_weights** (optional) - **T2**:
  New weights
* **__group_543__new_gradients** (optional) - **T3**:
  New gradients
* **__group_543__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_543__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_543__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_544__new_weights** (optional) - **T2**:
  New weights
* **__group_544__new_gradients** (optional) - **T3**:
  New gradients
* **__group_544__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_544__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_544__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_545__new_weights** (optional) - **T2**:
  New weights
* **__group_545__new_gradients** (optional) - **T3**:
  New gradients
* **__group_545__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_545__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_545__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_546__new_weights** (optional) - **T2**:
  New weights
* **__group_546__new_gradients** (optional) - **T3**:
  New gradients
* **__group_546__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_546__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_546__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_547__new_weights** (optional) - **T2**:
  New weights
* **__group_547__new_gradients** (optional) - **T3**:
  New gradients
* **__group_547__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_547__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_547__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_548__new_weights** (optional) - **T2**:
  New weights
* **__group_548__new_gradients** (optional) - **T3**:
  New gradients
* **__group_548__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_548__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_548__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_549__new_weights** (optional) - **T2**:
  New weights
* **__group_549__new_gradients** (optional) - **T3**:
  New gradients
* **__group_549__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_549__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_549__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_550__new_weights** (optional) - **T2**:
  New weights
* **__group_550__new_gradients** (optional) - **T3**:
  New gradients
* **__group_550__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_550__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_550__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_551__new_weights** (optional) - **T2**:
  New weights
* **__group_551__new_gradients** (optional) - **T3**:
  New gradients
* **__group_551__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_551__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_551__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_552__new_weights** (optional) - **T2**:
  New weights
* **__group_552__new_gradients** (optional) - **T3**:
  New gradients
* **__group_552__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_552__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_552__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_553__new_weights** (optional) - **T2**:
  New weights
* **__group_553__new_gradients** (optional) - **T3**:
  New gradients
* **__group_553__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_553__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_553__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_554__new_weights** (optional) - **T2**:
  New weights
* **__group_554__new_gradients** (optional) - **T3**:
  New gradients
* **__group_554__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_554__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_554__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_555__new_weights** (optional) - **T2**:
  New weights
* **__group_555__new_gradients** (optional) - **T3**:
  New gradients
* **__group_555__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_555__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_555__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_556__new_weights** (optional) - **T2**:
  New weights
* **__group_556__new_gradients** (optional) - **T3**:
  New gradients
* **__group_556__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_556__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_556__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_557__new_weights** (optional) - **T2**:
  New weights
* **__group_557__new_gradients** (optional) - **T3**:
  New gradients
* **__group_557__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_557__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_557__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_558__new_weights** (optional) - **T2**:
  New weights
* **__group_558__new_gradients** (optional) - **T3**:
  New gradients
* **__group_558__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_558__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_558__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_559__new_weights** (optional) - **T2**:
  New weights
* **__group_559__new_gradients** (optional) - **T3**:
  New gradients
* **__group_559__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_559__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_559__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_560__new_weights** (optional) - **T2**:
  New weights
* **__group_560__new_gradients** (optional) - **T3**:
  New gradients
* **__group_560__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_560__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_560__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_561__new_weights** (optional) - **T2**:
  New weights
* **__group_561__new_gradients** (optional) - **T3**:
  New gradients
* **__group_561__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_561__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_561__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_562__new_weights** (optional) - **T2**:
  New weights
* **__group_562__new_gradients** (optional) - **T3**:
  New gradients
* **__group_562__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_562__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_562__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_563__new_weights** (optional) - **T2**:
  New weights
* **__group_563__new_gradients** (optional) - **T3**:
  New gradients
* **__group_563__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_563__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_563__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_564__new_weights** (optional) - **T2**:
  New weights
* **__group_564__new_gradients** (optional) - **T3**:
  New gradients
* **__group_564__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_564__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_564__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_565__new_weights** (optional) - **T2**:
  New weights
* **__group_565__new_gradients** (optional) - **T3**:
  New gradients
* **__group_565__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_565__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_565__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_566__new_weights** (optional) - **T2**:
  New weights
* **__group_566__new_gradients** (optional) - **T3**:
  New gradients
* **__group_566__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_566__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_566__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_567__new_weights** (optional) - **T2**:
  New weights
* **__group_567__new_gradients** (optional) - **T3**:
  New gradients
* **__group_567__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_567__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_567__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_568__new_weights** (optional) - **T2**:
  New weights
* **__group_568__new_gradients** (optional) - **T3**:
  New gradients
* **__group_568__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_568__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_568__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_569__new_weights** (optional) - **T2**:
  New weights
* **__group_569__new_gradients** (optional) - **T3**:
  New gradients
* **__group_569__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_569__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_569__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_570__new_weights** (optional) - **T2**:
  New weights
* **__group_570__new_gradients** (optional) - **T3**:
  New gradients
* **__group_570__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_570__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_570__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_571__new_weights** (optional) - **T2**:
  New weights
* **__group_571__new_gradients** (optional) - **T3**:
  New gradients
* **__group_571__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_571__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_571__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_572__new_weights** (optional) - **T2**:
  New weights
* **__group_572__new_gradients** (optional) - **T3**:
  New gradients
* **__group_572__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_572__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_572__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_573__new_weights** (optional) - **T2**:
  New weights
* **__group_573__new_gradients** (optional) - **T3**:
  New gradients
* **__group_573__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_573__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_573__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_574__new_weights** (optional) - **T2**:
  New weights
* **__group_574__new_gradients** (optional) - **T3**:
  New gradients
* **__group_574__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_574__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_574__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_575__new_weights** (optional) - **T2**:
  New weights
* **__group_575__new_gradients** (optional) - **T3**:
  New gradients
* **__group_575__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_575__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_575__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_576__new_weights** (optional) - **T2**:
  New weights
* **__group_576__new_gradients** (optional) - **T3**:
  New gradients
* **__group_576__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_576__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_576__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_577__new_weights** (optional) - **T2**:
  New weights
* **__group_577__new_gradients** (optional) - **T3**:
  New gradients
* **__group_577__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_577__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_577__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_578__new_weights** (optional) - **T2**:
  New weights
* **__group_578__new_gradients** (optional) - **T3**:
  New gradients
* **__group_578__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_578__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_578__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_579__new_weights** (optional) - **T2**:
  New weights
* **__group_579__new_gradients** (optional) - **T3**:
  New gradients
* **__group_579__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_579__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_579__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_580__new_weights** (optional) - **T2**:
  New weights
* **__group_580__new_gradients** (optional) - **T3**:
  New gradients
* **__group_580__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_580__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_580__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_581__new_weights** (optional) - **T2**:
  New weights
* **__group_581__new_gradients** (optional) - **T3**:
  New gradients
* **__group_581__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_581__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_581__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_582__new_weights** (optional) - **T2**:
  New weights
* **__group_582__new_gradients** (optional) - **T3**:
  New gradients
* **__group_582__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_582__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_582__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_583__new_weights** (optional) - **T2**:
  New weights
* **__group_583__new_gradients** (optional) - **T3**:
  New gradients
* **__group_583__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_583__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_583__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_584__new_weights** (optional) - **T2**:
  New weights
* **__group_584__new_gradients** (optional) - **T3**:
  New gradients
* **__group_584__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_584__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_584__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_585__new_weights** (optional) - **T2**:
  New weights
* **__group_585__new_gradients** (optional) - **T3**:
  New gradients
* **__group_585__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_585__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_585__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_586__new_weights** (optional) - **T2**:
  New weights
* **__group_586__new_gradients** (optional) - **T3**:
  New gradients
* **__group_586__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_586__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_586__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_587__new_weights** (optional) - **T2**:
  New weights
* **__group_587__new_gradients** (optional) - **T3**:
  New gradients
* **__group_587__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_587__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_587__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_588__new_weights** (optional) - **T2**:
  New weights
* **__group_588__new_gradients** (optional) - **T3**:
  New gradients
* **__group_588__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_588__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_588__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_589__new_weights** (optional) - **T2**:
  New weights
* **__group_589__new_gradients** (optional) - **T3**:
  New gradients
* **__group_589__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_589__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_589__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_590__new_weights** (optional) - **T2**:
  New weights
* **__group_590__new_gradients** (optional) - **T3**:
  New gradients
* **__group_590__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_590__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_590__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_591__new_weights** (optional) - **T2**:
  New weights
* **__group_591__new_gradients** (optional) - **T3**:
  New gradients
* **__group_591__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_591__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_591__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_592__new_weights** (optional) - **T2**:
  New weights
* **__group_592__new_gradients** (optional) - **T3**:
  New gradients
* **__group_592__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_592__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_592__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_593__new_weights** (optional) - **T2**:
  New weights
* **__group_593__new_gradients** (optional) - **T3**:
  New gradients
* **__group_593__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_593__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_593__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_594__new_weights** (optional) - **T2**:
  New weights
* **__group_594__new_gradients** (optional) - **T3**:
  New gradients
* **__group_594__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_594__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_594__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_595__new_weights** (optional) - **T2**:
  New weights
* **__group_595__new_gradients** (optional) - **T3**:
  New gradients
* **__group_595__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_595__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_595__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_596__new_weights** (optional) - **T2**:
  New weights
* **__group_596__new_gradients** (optional) - **T3**:
  New gradients
* **__group_596__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_596__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_596__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_597__new_weights** (optional) - **T2**:
  New weights
* **__group_597__new_gradients** (optional) - **T3**:
  New gradients
* **__group_597__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_597__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_597__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_598__new_weights** (optional) - **T2**:
  New weights
* **__group_598__new_gradients** (optional) - **T3**:
  New gradients
* **__group_598__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_598__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_598__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_599__new_weights** (optional) - **T2**:
  New weights
* **__group_599__new_gradients** (optional) - **T3**:
  New gradients
* **__group_599__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_599__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_599__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_600__new_weights** (optional) - **T2**:
  New weights
* **__group_600__new_gradients** (optional) - **T3**:
  New gradients
* **__group_600__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_600__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_600__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_601__new_weights** (optional) - **T2**:
  New weights
* **__group_601__new_gradients** (optional) - **T3**:
  New gradients
* **__group_601__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_601__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_601__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_602__new_weights** (optional) - **T2**:
  New weights
* **__group_602__new_gradients** (optional) - **T3**:
  New gradients
* **__group_602__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_602__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_602__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_603__new_weights** (optional) - **T2**:
  New weights
* **__group_603__new_gradients** (optional) - **T3**:
  New gradients
* **__group_603__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_603__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_603__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_604__new_weights** (optional) - **T2**:
  New weights
* **__group_604__new_gradients** (optional) - **T3**:
  New gradients
* **__group_604__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_604__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_604__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_605__new_weights** (optional) - **T2**:
  New weights
* **__group_605__new_gradients** (optional) - **T3**:
  New gradients
* **__group_605__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_605__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_605__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_606__new_weights** (optional) - **T2**:
  New weights
* **__group_606__new_gradients** (optional) - **T3**:
  New gradients
* **__group_606__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_606__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_606__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_607__new_weights** (optional) - **T2**:
  New weights
* **__group_607__new_gradients** (optional) - **T3**:
  New gradients
* **__group_607__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_607__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_607__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_608__new_weights** (optional) - **T2**:
  New weights
* **__group_608__new_gradients** (optional) - **T3**:
  New gradients
* **__group_608__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_608__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_608__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_609__new_weights** (optional) - **T2**:
  New weights
* **__group_609__new_gradients** (optional) - **T3**:
  New gradients
* **__group_609__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_609__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_609__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_610__new_weights** (optional) - **T2**:
  New weights
* **__group_610__new_gradients** (optional) - **T3**:
  New gradients
* **__group_610__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_610__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_610__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_611__new_weights** (optional) - **T2**:
  New weights
* **__group_611__new_gradients** (optional) - **T3**:
  New gradients
* **__group_611__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_611__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_611__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_612__new_weights** (optional) - **T2**:
  New weights
* **__group_612__new_gradients** (optional) - **T3**:
  New gradients
* **__group_612__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_612__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_612__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_613__new_weights** (optional) - **T2**:
  New weights
* **__group_613__new_gradients** (optional) - **T3**:
  New gradients
* **__group_613__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_613__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_613__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_614__new_weights** (optional) - **T2**:
  New weights
* **__group_614__new_gradients** (optional) - **T3**:
  New gradients
* **__group_614__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_614__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_614__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_615__new_weights** (optional) - **T2**:
  New weights
* **__group_615__new_gradients** (optional) - **T3**:
  New gradients
* **__group_615__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_615__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_615__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_616__new_weights** (optional) - **T2**:
  New weights
* **__group_616__new_gradients** (optional) - **T3**:
  New gradients
* **__group_616__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_616__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_616__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_617__new_weights** (optional) - **T2**:
  New weights
* **__group_617__new_gradients** (optional) - **T3**:
  New gradients
* **__group_617__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_617__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_617__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_618__new_weights** (optional) - **T2**:
  New weights
* **__group_618__new_gradients** (optional) - **T3**:
  New gradients
* **__group_618__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_618__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_618__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_619__new_weights** (optional) - **T2**:
  New weights
* **__group_619__new_gradients** (optional) - **T3**:
  New gradients
* **__group_619__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_619__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_619__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_620__new_weights** (optional) - **T2**:
  New weights
* **__group_620__new_gradients** (optional) - **T3**:
  New gradients
* **__group_620__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_620__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_620__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_621__new_weights** (optional) - **T2**:
  New weights
* **__group_621__new_gradients** (optional) - **T3**:
  New gradients
* **__group_621__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_621__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_621__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_622__new_weights** (optional) - **T2**:
  New weights
* **__group_622__new_gradients** (optional) - **T3**:
  New gradients
* **__group_622__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_622__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_622__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_623__new_weights** (optional) - **T2**:
  New weights
* **__group_623__new_gradients** (optional) - **T3**:
  New gradients
* **__group_623__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_623__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_623__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_624__new_weights** (optional) - **T2**:
  New weights
* **__group_624__new_gradients** (optional) - **T3**:
  New gradients
* **__group_624__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_624__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_624__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_625__new_weights** (optional) - **T2**:
  New weights
* **__group_625__new_gradients** (optional) - **T3**:
  New gradients
* **__group_625__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_625__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_625__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_626__new_weights** (optional) - **T2**:
  New weights
* **__group_626__new_gradients** (optional) - **T3**:
  New gradients
* **__group_626__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_626__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_626__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_627__new_weights** (optional) - **T2**:
  New weights
* **__group_627__new_gradients** (optional) - **T3**:
  New gradients
* **__group_627__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_627__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_627__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_628__new_weights** (optional) - **T2**:
  New weights
* **__group_628__new_gradients** (optional) - **T3**:
  New gradients
* **__group_628__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_628__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_628__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_629__new_weights** (optional) - **T2**:
  New weights
* **__group_629__new_gradients** (optional) - **T3**:
  New gradients
* **__group_629__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_629__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_629__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_630__new_weights** (optional) - **T2**:
  New weights
* **__group_630__new_gradients** (optional) - **T3**:
  New gradients
* **__group_630__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_630__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_630__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_631__new_weights** (optional) - **T2**:
  New weights
* **__group_631__new_gradients** (optional) - **T3**:
  New gradients
* **__group_631__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_631__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_631__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_632__new_weights** (optional) - **T2**:
  New weights
* **__group_632__new_gradients** (optional) - **T3**:
  New gradients
* **__group_632__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_632__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_632__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_633__new_weights** (optional) - **T2**:
  New weights
* **__group_633__new_gradients** (optional) - **T3**:
  New gradients
* **__group_633__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_633__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_633__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_634__new_weights** (optional) - **T2**:
  New weights
* **__group_634__new_gradients** (optional) - **T3**:
  New gradients
* **__group_634__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_634__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_634__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_635__new_weights** (optional) - **T2**:
  New weights
* **__group_635__new_gradients** (optional) - **T3**:
  New gradients
* **__group_635__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_635__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_635__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_636__new_weights** (optional) - **T2**:
  New weights
* **__group_636__new_gradients** (optional) - **T3**:
  New gradients
* **__group_636__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_636__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_636__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_637__new_weights** (optional) - **T2**:
  New weights
* **__group_637__new_gradients** (optional) - **T3**:
  New gradients
* **__group_637__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_637__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_637__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_638__new_weights** (optional) - **T2**:
  New weights
* **__group_638__new_gradients** (optional) - **T3**:
  New gradients
* **__group_638__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_638__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_638__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_639__new_weights** (optional) - **T2**:
  New weights
* **__group_639__new_gradients** (optional) - **T3**:
  New gradients
* **__group_639__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_639__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_639__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_640__new_weights** (optional) - **T2**:
  New weights
* **__group_640__new_gradients** (optional) - **T3**:
  New gradients
* **__group_640__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_640__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_640__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_641__new_weights** (optional) - **T2**:
  New weights
* **__group_641__new_gradients** (optional) - **T3**:
  New gradients
* **__group_641__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_641__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_641__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_642__new_weights** (optional) - **T2**:
  New weights
* **__group_642__new_gradients** (optional) - **T3**:
  New gradients
* **__group_642__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_642__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_642__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_643__new_weights** (optional) - **T2**:
  New weights
* **__group_643__new_gradients** (optional) - **T3**:
  New gradients
* **__group_643__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_643__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_643__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_644__new_weights** (optional) - **T2**:
  New weights
* **__group_644__new_gradients** (optional) - **T3**:
  New gradients
* **__group_644__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_644__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_644__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_645__new_weights** (optional) - **T2**:
  New weights
* **__group_645__new_gradients** (optional) - **T3**:
  New gradients
* **__group_645__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_645__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_645__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_646__new_weights** (optional) - **T2**:
  New weights
* **__group_646__new_gradients** (optional) - **T3**:
  New gradients
* **__group_646__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_646__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_646__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_647__new_weights** (optional) - **T2**:
  New weights
* **__group_647__new_gradients** (optional) - **T3**:
  New gradients
* **__group_647__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_647__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_647__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_648__new_weights** (optional) - **T2**:
  New weights
* **__group_648__new_gradients** (optional) - **T3**:
  New gradients
* **__group_648__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_648__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_648__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_649__new_weights** (optional) - **T2**:
  New weights
* **__group_649__new_gradients** (optional) - **T3**:
  New gradients
* **__group_649__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_649__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_649__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_650__new_weights** (optional) - **T2**:
  New weights
* **__group_650__new_gradients** (optional) - **T3**:
  New gradients
* **__group_650__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_650__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_650__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_651__new_weights** (optional) - **T2**:
  New weights
* **__group_651__new_gradients** (optional) - **T3**:
  New gradients
* **__group_651__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_651__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_651__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_652__new_weights** (optional) - **T2**:
  New weights
* **__group_652__new_gradients** (optional) - **T3**:
  New gradients
* **__group_652__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_652__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_652__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_653__new_weights** (optional) - **T2**:
  New weights
* **__group_653__new_gradients** (optional) - **T3**:
  New gradients
* **__group_653__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_653__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_653__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_654__new_weights** (optional) - **T2**:
  New weights
* **__group_654__new_gradients** (optional) - **T3**:
  New gradients
* **__group_654__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_654__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_654__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_655__new_weights** (optional) - **T2**:
  New weights
* **__group_655__new_gradients** (optional) - **T3**:
  New gradients
* **__group_655__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_655__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_655__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_656__new_weights** (optional) - **T2**:
  New weights
* **__group_656__new_gradients** (optional) - **T3**:
  New gradients
* **__group_656__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_656__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_656__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_657__new_weights** (optional) - **T2**:
  New weights
* **__group_657__new_gradients** (optional) - **T3**:
  New gradients
* **__group_657__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_657__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_657__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_658__new_weights** (optional) - **T2**:
  New weights
* **__group_658__new_gradients** (optional) - **T3**:
  New gradients
* **__group_658__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_658__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_658__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_659__new_weights** (optional) - **T2**:
  New weights
* **__group_659__new_gradients** (optional) - **T3**:
  New gradients
* **__group_659__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_659__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_659__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_660__new_weights** (optional) - **T2**:
  New weights
* **__group_660__new_gradients** (optional) - **T3**:
  New gradients
* **__group_660__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_660__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_660__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_661__new_weights** (optional) - **T2**:
  New weights
* **__group_661__new_gradients** (optional) - **T3**:
  New gradients
* **__group_661__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_661__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_661__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_662__new_weights** (optional) - **T2**:
  New weights
* **__group_662__new_gradients** (optional) - **T3**:
  New gradients
* **__group_662__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_662__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_662__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_663__new_weights** (optional) - **T2**:
  New weights
* **__group_663__new_gradients** (optional) - **T3**:
  New gradients
* **__group_663__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_663__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_663__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_664__new_weights** (optional) - **T2**:
  New weights
* **__group_664__new_gradients** (optional) - **T3**:
  New gradients
* **__group_664__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_664__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_664__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_665__new_weights** (optional) - **T2**:
  New weights
* **__group_665__new_gradients** (optional) - **T3**:
  New gradients
* **__group_665__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_665__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_665__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_666__new_weights** (optional) - **T2**:
  New weights
* **__group_666__new_gradients** (optional) - **T3**:
  New gradients
* **__group_666__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_666__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_666__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_667__new_weights** (optional) - **T2**:
  New weights
* **__group_667__new_gradients** (optional) - **T3**:
  New gradients
* **__group_667__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_667__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_667__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_668__new_weights** (optional) - **T2**:
  New weights
* **__group_668__new_gradients** (optional) - **T3**:
  New gradients
* **__group_668__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_668__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_668__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_669__new_weights** (optional) - **T2**:
  New weights
* **__group_669__new_gradients** (optional) - **T3**:
  New gradients
* **__group_669__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_669__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_669__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_670__new_weights** (optional) - **T2**:
  New weights
* **__group_670__new_gradients** (optional) - **T3**:
  New gradients
* **__group_670__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_670__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_670__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_671__new_weights** (optional) - **T2**:
  New weights
* **__group_671__new_gradients** (optional) - **T3**:
  New gradients
* **__group_671__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_671__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_671__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_672__new_weights** (optional) - **T2**:
  New weights
* **__group_672__new_gradients** (optional) - **T3**:
  New gradients
* **__group_672__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_672__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_672__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_673__new_weights** (optional) - **T2**:
  New weights
* **__group_673__new_gradients** (optional) - **T3**:
  New gradients
* **__group_673__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_673__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_673__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_674__new_weights** (optional) - **T2**:
  New weights
* **__group_674__new_gradients** (optional) - **T3**:
  New gradients
* **__group_674__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_674__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_674__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_675__new_weights** (optional) - **T2**:
  New weights
* **__group_675__new_gradients** (optional) - **T3**:
  New gradients
* **__group_675__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_675__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_675__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_676__new_weights** (optional) - **T2**:
  New weights
* **__group_676__new_gradients** (optional) - **T3**:
  New gradients
* **__group_676__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_676__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_676__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_677__new_weights** (optional) - **T2**:
  New weights
* **__group_677__new_gradients** (optional) - **T3**:
  New gradients
* **__group_677__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_677__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_677__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_678__new_weights** (optional) - **T2**:
  New weights
* **__group_678__new_gradients** (optional) - **T3**:
  New gradients
* **__group_678__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_678__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_678__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_679__new_weights** (optional) - **T2**:
  New weights
* **__group_679__new_gradients** (optional) - **T3**:
  New gradients
* **__group_679__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_679__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_679__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_680__new_weights** (optional) - **T2**:
  New weights
* **__group_680__new_gradients** (optional) - **T3**:
  New gradients
* **__group_680__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_680__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_680__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_681__new_weights** (optional) - **T2**:
  New weights
* **__group_681__new_gradients** (optional) - **T3**:
  New gradients
* **__group_681__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_681__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_681__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_682__new_weights** (optional) - **T2**:
  New weights
* **__group_682__new_gradients** (optional) - **T3**:
  New gradients
* **__group_682__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_682__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_682__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_683__new_weights** (optional) - **T2**:
  New weights
* **__group_683__new_gradients** (optional) - **T3**:
  New gradients
* **__group_683__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_683__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_683__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_684__new_weights** (optional) - **T2**:
  New weights
* **__group_684__new_gradients** (optional) - **T3**:
  New gradients
* **__group_684__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_684__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_684__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_685__new_weights** (optional) - **T2**:
  New weights
* **__group_685__new_gradients** (optional) - **T3**:
  New gradients
* **__group_685__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_685__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_685__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_686__new_weights** (optional) - **T2**:
  New weights
* **__group_686__new_gradients** (optional) - **T3**:
  New gradients
* **__group_686__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_686__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_686__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_687__new_weights** (optional) - **T2**:
  New weights
* **__group_687__new_gradients** (optional) - **T3**:
  New gradients
* **__group_687__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_687__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_687__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_688__new_weights** (optional) - **T2**:
  New weights
* **__group_688__new_gradients** (optional) - **T3**:
  New gradients
* **__group_688__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_688__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_688__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_689__new_weights** (optional) - **T2**:
  New weights
* **__group_689__new_gradients** (optional) - **T3**:
  New gradients
* **__group_689__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_689__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_689__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_690__new_weights** (optional) - **T2**:
  New weights
* **__group_690__new_gradients** (optional) - **T3**:
  New gradients
* **__group_690__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_690__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_690__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_691__new_weights** (optional) - **T2**:
  New weights
* **__group_691__new_gradients** (optional) - **T3**:
  New gradients
* **__group_691__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_691__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_691__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_692__new_weights** (optional) - **T2**:
  New weights
* **__group_692__new_gradients** (optional) - **T3**:
  New gradients
* **__group_692__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_692__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_692__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_693__new_weights** (optional) - **T2**:
  New weights
* **__group_693__new_gradients** (optional) - **T3**:
  New gradients
* **__group_693__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_693__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_693__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_694__new_weights** (optional) - **T2**:
  New weights
* **__group_694__new_gradients** (optional) - **T3**:
  New gradients
* **__group_694__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_694__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_694__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_695__new_weights** (optional) - **T2**:
  New weights
* **__group_695__new_gradients** (optional) - **T3**:
  New gradients
* **__group_695__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_695__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_695__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_696__new_weights** (optional) - **T2**:
  New weights
* **__group_696__new_gradients** (optional) - **T3**:
  New gradients
* **__group_696__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_696__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_696__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_697__new_weights** (optional) - **T2**:
  New weights
* **__group_697__new_gradients** (optional) - **T3**:
  New gradients
* **__group_697__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_697__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_697__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_698__new_weights** (optional) - **T2**:
  New weights
* **__group_698__new_gradients** (optional) - **T3**:
  New gradients
* **__group_698__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_698__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_698__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_699__new_weights** (optional) - **T2**:
  New weights
* **__group_699__new_gradients** (optional) - **T3**:
  New gradients
* **__group_699__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_699__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_699__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_700__new_weights** (optional) - **T2**:
  New weights
* **__group_700__new_gradients** (optional) - **T3**:
  New gradients
* **__group_700__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_700__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_700__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_701__new_weights** (optional) - **T2**:
  New weights
* **__group_701__new_gradients** (optional) - **T3**:
  New gradients
* **__group_701__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_701__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_701__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_702__new_weights** (optional) - **T2**:
  New weights
* **__group_702__new_gradients** (optional) - **T3**:
  New gradients
* **__group_702__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_702__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_702__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_703__new_weights** (optional) - **T2**:
  New weights
* **__group_703__new_gradients** (optional) - **T3**:
  New gradients
* **__group_703__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_703__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_703__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_704__new_weights** (optional) - **T2**:
  New weights
* **__group_704__new_gradients** (optional) - **T3**:
  New gradients
* **__group_704__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_704__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_704__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_705__new_weights** (optional) - **T2**:
  New weights
* **__group_705__new_gradients** (optional) - **T3**:
  New gradients
* **__group_705__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_705__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_705__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_706__new_weights** (optional) - **T2**:
  New weights
* **__group_706__new_gradients** (optional) - **T3**:
  New gradients
* **__group_706__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_706__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_706__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_707__new_weights** (optional) - **T2**:
  New weights
* **__group_707__new_gradients** (optional) - **T3**:
  New gradients
* **__group_707__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_707__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_707__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_708__new_weights** (optional) - **T2**:
  New weights
* **__group_708__new_gradients** (optional) - **T3**:
  New gradients
* **__group_708__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_708__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_708__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_709__new_weights** (optional) - **T2**:
  New weights
* **__group_709__new_gradients** (optional) - **T3**:
  New gradients
* **__group_709__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_709__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_709__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_710__new_weights** (optional) - **T2**:
  New weights
* **__group_710__new_gradients** (optional) - **T3**:
  New gradients
* **__group_710__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_710__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_710__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_711__new_weights** (optional) - **T2**:
  New weights
* **__group_711__new_gradients** (optional) - **T3**:
  New gradients
* **__group_711__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_711__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_711__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_712__new_weights** (optional) - **T2**:
  New weights
* **__group_712__new_gradients** (optional) - **T3**:
  New gradients
* **__group_712__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_712__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_712__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_713__new_weights** (optional) - **T2**:
  New weights
* **__group_713__new_gradients** (optional) - **T3**:
  New gradients
* **__group_713__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_713__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_713__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_714__new_weights** (optional) - **T2**:
  New weights
* **__group_714__new_gradients** (optional) - **T3**:
  New gradients
* **__group_714__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_714__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_714__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_715__new_weights** (optional) - **T2**:
  New weights
* **__group_715__new_gradients** (optional) - **T3**:
  New gradients
* **__group_715__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_715__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_715__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_716__new_weights** (optional) - **T2**:
  New weights
* **__group_716__new_gradients** (optional) - **T3**:
  New gradients
* **__group_716__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_716__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_716__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_717__new_weights** (optional) - **T2**:
  New weights
* **__group_717__new_gradients** (optional) - **T3**:
  New gradients
* **__group_717__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_717__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_717__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_718__new_weights** (optional) - **T2**:
  New weights
* **__group_718__new_gradients** (optional) - **T3**:
  New gradients
* **__group_718__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_718__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_718__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_719__new_weights** (optional) - **T2**:
  New weights
* **__group_719__new_gradients** (optional) - **T3**:
  New gradients
* **__group_719__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_719__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_719__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_720__new_weights** (optional) - **T2**:
  New weights
* **__group_720__new_gradients** (optional) - **T3**:
  New gradients
* **__group_720__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_720__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_720__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_721__new_weights** (optional) - **T2**:
  New weights
* **__group_721__new_gradients** (optional) - **T3**:
  New gradients
* **__group_721__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_721__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_721__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_722__new_weights** (optional) - **T2**:
  New weights
* **__group_722__new_gradients** (optional) - **T3**:
  New gradients
* **__group_722__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_722__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_722__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_723__new_weights** (optional) - **T2**:
  New weights
* **__group_723__new_gradients** (optional) - **T3**:
  New gradients
* **__group_723__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_723__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_723__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_724__new_weights** (optional) - **T2**:
  New weights
* **__group_724__new_gradients** (optional) - **T3**:
  New gradients
* **__group_724__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_724__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_724__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_725__new_weights** (optional) - **T2**:
  New weights
* **__group_725__new_gradients** (optional) - **T3**:
  New gradients
* **__group_725__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_725__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_725__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_726__new_weights** (optional) - **T2**:
  New weights
* **__group_726__new_gradients** (optional) - **T3**:
  New gradients
* **__group_726__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_726__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_726__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_727__new_weights** (optional) - **T2**:
  New weights
* **__group_727__new_gradients** (optional) - **T3**:
  New gradients
* **__group_727__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_727__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_727__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_728__new_weights** (optional) - **T2**:
  New weights
* **__group_728__new_gradients** (optional) - **T3**:
  New gradients
* **__group_728__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_728__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_728__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_729__new_weights** (optional) - **T2**:
  New weights
* **__group_729__new_gradients** (optional) - **T3**:
  New gradients
* **__group_729__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_729__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_729__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_730__new_weights** (optional) - **T2**:
  New weights
* **__group_730__new_gradients** (optional) - **T3**:
  New gradients
* **__group_730__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_730__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_730__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_731__new_weights** (optional) - **T2**:
  New weights
* **__group_731__new_gradients** (optional) - **T3**:
  New gradients
* **__group_731__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_731__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_731__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_732__new_weights** (optional) - **T2**:
  New weights
* **__group_732__new_gradients** (optional) - **T3**:
  New gradients
* **__group_732__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_732__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_732__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_733__new_weights** (optional) - **T2**:
  New weights
* **__group_733__new_gradients** (optional) - **T3**:
  New gradients
* **__group_733__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_733__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_733__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_734__new_weights** (optional) - **T2**:
  New weights
* **__group_734__new_gradients** (optional) - **T3**:
  New gradients
* **__group_734__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_734__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_734__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_735__new_weights** (optional) - **T2**:
  New weights
* **__group_735__new_gradients** (optional) - **T3**:
  New gradients
* **__group_735__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_735__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_735__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_736__new_weights** (optional) - **T2**:
  New weights
* **__group_736__new_gradients** (optional) - **T3**:
  New gradients
* **__group_736__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_736__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_736__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_737__new_weights** (optional) - **T2**:
  New weights
* **__group_737__new_gradients** (optional) - **T3**:
  New gradients
* **__group_737__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_737__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_737__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_738__new_weights** (optional) - **T2**:
  New weights
* **__group_738__new_gradients** (optional) - **T3**:
  New gradients
* **__group_738__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_738__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_738__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_739__new_weights** (optional) - **T2**:
  New weights
* **__group_739__new_gradients** (optional) - **T3**:
  New gradients
* **__group_739__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_739__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_739__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_740__new_weights** (optional) - **T2**:
  New weights
* **__group_740__new_gradients** (optional) - **T3**:
  New gradients
* **__group_740__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_740__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_740__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_741__new_weights** (optional) - **T2**:
  New weights
* **__group_741__new_gradients** (optional) - **T3**:
  New gradients
* **__group_741__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_741__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_741__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_742__new_weights** (optional) - **T2**:
  New weights
* **__group_742__new_gradients** (optional) - **T3**:
  New gradients
* **__group_742__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_742__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_742__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_743__new_weights** (optional) - **T2**:
  New weights
* **__group_743__new_gradients** (optional) - **T3**:
  New gradients
* **__group_743__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_743__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_743__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_744__new_weights** (optional) - **T2**:
  New weights
* **__group_744__new_gradients** (optional) - **T3**:
  New gradients
* **__group_744__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_744__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_744__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_745__new_weights** (optional) - **T2**:
  New weights
* **__group_745__new_gradients** (optional) - **T3**:
  New gradients
* **__group_745__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_745__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_745__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_746__new_weights** (optional) - **T2**:
  New weights
* **__group_746__new_gradients** (optional) - **T3**:
  New gradients
* **__group_746__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_746__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_746__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_747__new_weights** (optional) - **T2**:
  New weights
* **__group_747__new_gradients** (optional) - **T3**:
  New gradients
* **__group_747__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_747__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_747__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_748__new_weights** (optional) - **T2**:
  New weights
* **__group_748__new_gradients** (optional) - **T3**:
  New gradients
* **__group_748__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_748__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_748__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_749__new_weights** (optional) - **T2**:
  New weights
* **__group_749__new_gradients** (optional) - **T3**:
  New gradients
* **__group_749__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_749__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_749__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_750__new_weights** (optional) - **T2**:
  New weights
* **__group_750__new_gradients** (optional) - **T3**:
  New gradients
* **__group_750__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_750__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_750__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_751__new_weights** (optional) - **T2**:
  New weights
* **__group_751__new_gradients** (optional) - **T3**:
  New gradients
* **__group_751__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_751__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_751__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_752__new_weights** (optional) - **T2**:
  New weights
* **__group_752__new_gradients** (optional) - **T3**:
  New gradients
* **__group_752__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_752__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_752__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_753__new_weights** (optional) - **T2**:
  New weights
* **__group_753__new_gradients** (optional) - **T3**:
  New gradients
* **__group_753__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_753__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_753__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_754__new_weights** (optional) - **T2**:
  New weights
* **__group_754__new_gradients** (optional) - **T3**:
  New gradients
* **__group_754__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_754__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_754__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_755__new_weights** (optional) - **T2**:
  New weights
* **__group_755__new_gradients** (optional) - **T3**:
  New gradients
* **__group_755__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_755__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_755__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_756__new_weights** (optional) - **T2**:
  New weights
* **__group_756__new_gradients** (optional) - **T3**:
  New gradients
* **__group_756__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_756__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_756__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_757__new_weights** (optional) - **T2**:
  New weights
* **__group_757__new_gradients** (optional) - **T3**:
  New gradients
* **__group_757__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_757__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_757__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_758__new_weights** (optional) - **T2**:
  New weights
* **__group_758__new_gradients** (optional) - **T3**:
  New gradients
* **__group_758__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_758__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_758__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_759__new_weights** (optional) - **T2**:
  New weights
* **__group_759__new_gradients** (optional) - **T3**:
  New gradients
* **__group_759__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_759__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_759__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_760__new_weights** (optional) - **T2**:
  New weights
* **__group_760__new_gradients** (optional) - **T3**:
  New gradients
* **__group_760__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_760__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_760__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_761__new_weights** (optional) - **T2**:
  New weights
* **__group_761__new_gradients** (optional) - **T3**:
  New gradients
* **__group_761__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_761__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_761__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_762__new_weights** (optional) - **T2**:
  New weights
* **__group_762__new_gradients** (optional) - **T3**:
  New gradients
* **__group_762__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_762__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_762__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_763__new_weights** (optional) - **T2**:
  New weights
* **__group_763__new_gradients** (optional) - **T3**:
  New gradients
* **__group_763__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_763__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_763__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_764__new_weights** (optional) - **T2**:
  New weights
* **__group_764__new_gradients** (optional) - **T3**:
  New gradients
* **__group_764__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_764__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_764__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_765__new_weights** (optional) - **T2**:
  New weights
* **__group_765__new_gradients** (optional) - **T3**:
  New gradients
* **__group_765__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_765__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_765__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_766__new_weights** (optional) - **T2**:
  New weights
* **__group_766__new_gradients** (optional) - **T3**:
  New gradients
* **__group_766__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_766__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_766__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_767__new_weights** (optional) - **T2**:
  New weights
* **__group_767__new_gradients** (optional) - **T3**:
  New gradients
* **__group_767__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_767__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_767__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_768__new_weights** (optional) - **T2**:
  New weights
* **__group_768__new_gradients** (optional) - **T3**:
  New gradients
* **__group_768__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_768__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_768__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_769__new_weights** (optional) - **T2**:
  New weights
* **__group_769__new_gradients** (optional) - **T3**:
  New gradients
* **__group_769__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_769__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_769__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_770__new_weights** (optional) - **T2**:
  New weights
* **__group_770__new_gradients** (optional) - **T3**:
  New gradients
* **__group_770__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_770__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_770__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_771__new_weights** (optional) - **T2**:
  New weights
* **__group_771__new_gradients** (optional) - **T3**:
  New gradients
* **__group_771__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_771__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_771__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_772__new_weights** (optional) - **T2**:
  New weights
* **__group_772__new_gradients** (optional) - **T3**:
  New gradients
* **__group_772__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_772__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_772__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_773__new_weights** (optional) - **T2**:
  New weights
* **__group_773__new_gradients** (optional) - **T3**:
  New gradients
* **__group_773__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_773__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_773__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_774__new_weights** (optional) - **T2**:
  New weights
* **__group_774__new_gradients** (optional) - **T3**:
  New gradients
* **__group_774__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_774__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_774__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_775__new_weights** (optional) - **T2**:
  New weights
* **__group_775__new_gradients** (optional) - **T3**:
  New gradients
* **__group_775__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_775__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_775__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_776__new_weights** (optional) - **T2**:
  New weights
* **__group_776__new_gradients** (optional) - **T3**:
  New gradients
* **__group_776__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_776__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_776__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_777__new_weights** (optional) - **T2**:
  New weights
* **__group_777__new_gradients** (optional) - **T3**:
  New gradients
* **__group_777__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_777__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_777__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_778__new_weights** (optional) - **T2**:
  New weights
* **__group_778__new_gradients** (optional) - **T3**:
  New gradients
* **__group_778__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_778__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_778__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_779__new_weights** (optional) - **T2**:
  New weights
* **__group_779__new_gradients** (optional) - **T3**:
  New gradients
* **__group_779__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_779__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_779__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_780__new_weights** (optional) - **T2**:
  New weights
* **__group_780__new_gradients** (optional) - **T3**:
  New gradients
* **__group_780__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_780__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_780__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_781__new_weights** (optional) - **T2**:
  New weights
* **__group_781__new_gradients** (optional) - **T3**:
  New gradients
* **__group_781__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_781__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_781__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_782__new_weights** (optional) - **T2**:
  New weights
* **__group_782__new_gradients** (optional) - **T3**:
  New gradients
* **__group_782__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_782__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_782__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_783__new_weights** (optional) - **T2**:
  New weights
* **__group_783__new_gradients** (optional) - **T3**:
  New gradients
* **__group_783__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_783__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_783__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_784__new_weights** (optional) - **T2**:
  New weights
* **__group_784__new_gradients** (optional) - **T3**:
  New gradients
* **__group_784__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_784__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_784__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_785__new_weights** (optional) - **T2**:
  New weights
* **__group_785__new_gradients** (optional) - **T3**:
  New gradients
* **__group_785__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_785__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_785__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_786__new_weights** (optional) - **T2**:
  New weights
* **__group_786__new_gradients** (optional) - **T3**:
  New gradients
* **__group_786__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_786__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_786__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_787__new_weights** (optional) - **T2**:
  New weights
* **__group_787__new_gradients** (optional) - **T3**:
  New gradients
* **__group_787__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_787__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_787__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_788__new_weights** (optional) - **T2**:
  New weights
* **__group_788__new_gradients** (optional) - **T3**:
  New gradients
* **__group_788__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_788__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_788__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_789__new_weights** (optional) - **T2**:
  New weights
* **__group_789__new_gradients** (optional) - **T3**:
  New gradients
* **__group_789__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_789__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_789__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_790__new_weights** (optional) - **T2**:
  New weights
* **__group_790__new_gradients** (optional) - **T3**:
  New gradients
* **__group_790__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_790__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_790__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_791__new_weights** (optional) - **T2**:
  New weights
* **__group_791__new_gradients** (optional) - **T3**:
  New gradients
* **__group_791__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_791__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_791__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_792__new_weights** (optional) - **T2**:
  New weights
* **__group_792__new_gradients** (optional) - **T3**:
  New gradients
* **__group_792__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_792__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_792__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_793__new_weights** (optional) - **T2**:
  New weights
* **__group_793__new_gradients** (optional) - **T3**:
  New gradients
* **__group_793__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_793__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_793__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_794__new_weights** (optional) - **T2**:
  New weights
* **__group_794__new_gradients** (optional) - **T3**:
  New gradients
* **__group_794__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_794__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_794__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_795__new_weights** (optional) - **T2**:
  New weights
* **__group_795__new_gradients** (optional) - **T3**:
  New gradients
* **__group_795__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_795__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_795__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_796__new_weights** (optional) - **T2**:
  New weights
* **__group_796__new_gradients** (optional) - **T3**:
  New gradients
* **__group_796__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_796__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_796__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_797__new_weights** (optional) - **T2**:
  New weights
* **__group_797__new_gradients** (optional) - **T3**:
  New gradients
* **__group_797__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_797__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_797__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_798__new_weights** (optional) - **T2**:
  New weights
* **__group_798__new_gradients** (optional) - **T3**:
  New gradients
* **__group_798__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_798__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_798__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_799__new_weights** (optional) - **T2**:
  New weights
* **__group_799__new_gradients** (optional) - **T3**:
  New gradients
* **__group_799__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_799__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_799__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_800__new_weights** (optional) - **T2**:
  New weights
* **__group_800__new_gradients** (optional) - **T3**:
  New gradients
* **__group_800__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_800__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_800__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_801__new_weights** (optional) - **T2**:
  New weights
* **__group_801__new_gradients** (optional) - **T3**:
  New gradients
* **__group_801__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_801__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_801__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_802__new_weights** (optional) - **T2**:
  New weights
* **__group_802__new_gradients** (optional) - **T3**:
  New gradients
* **__group_802__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_802__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_802__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_803__new_weights** (optional) - **T2**:
  New weights
* **__group_803__new_gradients** (optional) - **T3**:
  New gradients
* **__group_803__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_803__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_803__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_804__new_weights** (optional) - **T2**:
  New weights
* **__group_804__new_gradients** (optional) - **T3**:
  New gradients
* **__group_804__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_804__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_804__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_805__new_weights** (optional) - **T2**:
  New weights
* **__group_805__new_gradients** (optional) - **T3**:
  New gradients
* **__group_805__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_805__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_805__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_806__new_weights** (optional) - **T2**:
  New weights
* **__group_806__new_gradients** (optional) - **T3**:
  New gradients
* **__group_806__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_806__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_806__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_807__new_weights** (optional) - **T2**:
  New weights
* **__group_807__new_gradients** (optional) - **T3**:
  New gradients
* **__group_807__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_807__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_807__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_808__new_weights** (optional) - **T2**:
  New weights
* **__group_808__new_gradients** (optional) - **T3**:
  New gradients
* **__group_808__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_808__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_808__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_809__new_weights** (optional) - **T2**:
  New weights
* **__group_809__new_gradients** (optional) - **T3**:
  New gradients
* **__group_809__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_809__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_809__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_810__new_weights** (optional) - **T2**:
  New weights
* **__group_810__new_gradients** (optional) - **T3**:
  New gradients
* **__group_810__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_810__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_810__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_811__new_weights** (optional) - **T2**:
  New weights
* **__group_811__new_gradients** (optional) - **T3**:
  New gradients
* **__group_811__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_811__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_811__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_812__new_weights** (optional) - **T2**:
  New weights
* **__group_812__new_gradients** (optional) - **T3**:
  New gradients
* **__group_812__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_812__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_812__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_813__new_weights** (optional) - **T2**:
  New weights
* **__group_813__new_gradients** (optional) - **T3**:
  New gradients
* **__group_813__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_813__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_813__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_814__new_weights** (optional) - **T2**:
  New weights
* **__group_814__new_gradients** (optional) - **T3**:
  New gradients
* **__group_814__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_814__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_814__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_815__new_weights** (optional) - **T2**:
  New weights
* **__group_815__new_gradients** (optional) - **T3**:
  New gradients
* **__group_815__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_815__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_815__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_816__new_weights** (optional) - **T2**:
  New weights
* **__group_816__new_gradients** (optional) - **T3**:
  New gradients
* **__group_816__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_816__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_816__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_817__new_weights** (optional) - **T2**:
  New weights
* **__group_817__new_gradients** (optional) - **T3**:
  New gradients
* **__group_817__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_817__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_817__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_818__new_weights** (optional) - **T2**:
  New weights
* **__group_818__new_gradients** (optional) - **T3**:
  New gradients
* **__group_818__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_818__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_818__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_819__new_weights** (optional) - **T2**:
  New weights
* **__group_819__new_gradients** (optional) - **T3**:
  New gradients
* **__group_819__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_819__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_819__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_820__new_weights** (optional) - **T2**:
  New weights
* **__group_820__new_gradients** (optional) - **T3**:
  New gradients
* **__group_820__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_820__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_820__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_821__new_weights** (optional) - **T2**:
  New weights
* **__group_821__new_gradients** (optional) - **T3**:
  New gradients
* **__group_821__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_821__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_821__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_822__new_weights** (optional) - **T2**:
  New weights
* **__group_822__new_gradients** (optional) - **T3**:
  New gradients
* **__group_822__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_822__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_822__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_823__new_weights** (optional) - **T2**:
  New weights
* **__group_823__new_gradients** (optional) - **T3**:
  New gradients
* **__group_823__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_823__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_823__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_824__new_weights** (optional) - **T2**:
  New weights
* **__group_824__new_gradients** (optional) - **T3**:
  New gradients
* **__group_824__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_824__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_824__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_825__new_weights** (optional) - **T2**:
  New weights
* **__group_825__new_gradients** (optional) - **T3**:
  New gradients
* **__group_825__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_825__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_825__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_826__new_weights** (optional) - **T2**:
  New weights
* **__group_826__new_gradients** (optional) - **T3**:
  New gradients
* **__group_826__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_826__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_826__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_827__new_weights** (optional) - **T2**:
  New weights
* **__group_827__new_gradients** (optional) - **T3**:
  New gradients
* **__group_827__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_827__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_827__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_828__new_weights** (optional) - **T2**:
  New weights
* **__group_828__new_gradients** (optional) - **T3**:
  New gradients
* **__group_828__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_828__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_828__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_829__new_weights** (optional) - **T2**:
  New weights
* **__group_829__new_gradients** (optional) - **T3**:
  New gradients
* **__group_829__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_829__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_829__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_830__new_weights** (optional) - **T2**:
  New weights
* **__group_830__new_gradients** (optional) - **T3**:
  New gradients
* **__group_830__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_830__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_830__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_831__new_weights** (optional) - **T2**:
  New weights
* **__group_831__new_gradients** (optional) - **T3**:
  New gradients
* **__group_831__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_831__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_831__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_832__new_weights** (optional) - **T2**:
  New weights
* **__group_832__new_gradients** (optional) - **T3**:
  New gradients
* **__group_832__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_832__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_832__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_833__new_weights** (optional) - **T2**:
  New weights
* **__group_833__new_gradients** (optional) - **T3**:
  New gradients
* **__group_833__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_833__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_833__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_834__new_weights** (optional) - **T2**:
  New weights
* **__group_834__new_gradients** (optional) - **T3**:
  New gradients
* **__group_834__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_834__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_834__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_835__new_weights** (optional) - **T2**:
  New weights
* **__group_835__new_gradients** (optional) - **T3**:
  New gradients
* **__group_835__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_835__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_835__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_836__new_weights** (optional) - **T2**:
  New weights
* **__group_836__new_gradients** (optional) - **T3**:
  New gradients
* **__group_836__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_836__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_836__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_837__new_weights** (optional) - **T2**:
  New weights
* **__group_837__new_gradients** (optional) - **T3**:
  New gradients
* **__group_837__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_837__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_837__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_838__new_weights** (optional) - **T2**:
  New weights
* **__group_838__new_gradients** (optional) - **T3**:
  New gradients
* **__group_838__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_838__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_838__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_839__new_weights** (optional) - **T2**:
  New weights
* **__group_839__new_gradients** (optional) - **T3**:
  New gradients
* **__group_839__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_839__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_839__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_840__new_weights** (optional) - **T2**:
  New weights
* **__group_840__new_gradients** (optional) - **T3**:
  New gradients
* **__group_840__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_840__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_840__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_841__new_weights** (optional) - **T2**:
  New weights
* **__group_841__new_gradients** (optional) - **T3**:
  New gradients
* **__group_841__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_841__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_841__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_842__new_weights** (optional) - **T2**:
  New weights
* **__group_842__new_gradients** (optional) - **T3**:
  New gradients
* **__group_842__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_842__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_842__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_843__new_weights** (optional) - **T2**:
  New weights
* **__group_843__new_gradients** (optional) - **T3**:
  New gradients
* **__group_843__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_843__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_843__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_844__new_weights** (optional) - **T2**:
  New weights
* **__group_844__new_gradients** (optional) - **T3**:
  New gradients
* **__group_844__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_844__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_844__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_845__new_weights** (optional) - **T2**:
  New weights
* **__group_845__new_gradients** (optional) - **T3**:
  New gradients
* **__group_845__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_845__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_845__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_846__new_weights** (optional) - **T2**:
  New weights
* **__group_846__new_gradients** (optional) - **T3**:
  New gradients
* **__group_846__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_846__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_846__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_847__new_weights** (optional) - **T2**:
  New weights
* **__group_847__new_gradients** (optional) - **T3**:
  New gradients
* **__group_847__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_847__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_847__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_848__new_weights** (optional) - **T2**:
  New weights
* **__group_848__new_gradients** (optional) - **T3**:
  New gradients
* **__group_848__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_848__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_848__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_849__new_weights** (optional) - **T2**:
  New weights
* **__group_849__new_gradients** (optional) - **T3**:
  New gradients
* **__group_849__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_849__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_849__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_850__new_weights** (optional) - **T2**:
  New weights
* **__group_850__new_gradients** (optional) - **T3**:
  New gradients
* **__group_850__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_850__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_850__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_851__new_weights** (optional) - **T2**:
  New weights
* **__group_851__new_gradients** (optional) - **T3**:
  New gradients
* **__group_851__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_851__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_851__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_852__new_weights** (optional) - **T2**:
  New weights
* **__group_852__new_gradients** (optional) - **T3**:
  New gradients
* **__group_852__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_852__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_852__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_853__new_weights** (optional) - **T2**:
  New weights
* **__group_853__new_gradients** (optional) - **T3**:
  New gradients
* **__group_853__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_853__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_853__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_854__new_weights** (optional) - **T2**:
  New weights
* **__group_854__new_gradients** (optional) - **T3**:
  New gradients
* **__group_854__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_854__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_854__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_855__new_weights** (optional) - **T2**:
  New weights
* **__group_855__new_gradients** (optional) - **T3**:
  New gradients
* **__group_855__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_855__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_855__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_856__new_weights** (optional) - **T2**:
  New weights
* **__group_856__new_gradients** (optional) - **T3**:
  New gradients
* **__group_856__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_856__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_856__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_857__new_weights** (optional) - **T2**:
  New weights
* **__group_857__new_gradients** (optional) - **T3**:
  New gradients
* **__group_857__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_857__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_857__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_858__new_weights** (optional) - **T2**:
  New weights
* **__group_858__new_gradients** (optional) - **T3**:
  New gradients
* **__group_858__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_858__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_858__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_859__new_weights** (optional) - **T2**:
  New weights
* **__group_859__new_gradients** (optional) - **T3**:
  New gradients
* **__group_859__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_859__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_859__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_860__new_weights** (optional) - **T2**:
  New weights
* **__group_860__new_gradients** (optional) - **T3**:
  New gradients
* **__group_860__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_860__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_860__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_861__new_weights** (optional) - **T2**:
  New weights
* **__group_861__new_gradients** (optional) - **T3**:
  New gradients
* **__group_861__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_861__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_861__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_862__new_weights** (optional) - **T2**:
  New weights
* **__group_862__new_gradients** (optional) - **T3**:
  New gradients
* **__group_862__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_862__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_862__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_863__new_weights** (optional) - **T2**:
  New weights
* **__group_863__new_gradients** (optional) - **T3**:
  New gradients
* **__group_863__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_863__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_863__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_864__new_weights** (optional) - **T2**:
  New weights
* **__group_864__new_gradients** (optional) - **T3**:
  New gradients
* **__group_864__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_864__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_864__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_865__new_weights** (optional) - **T2**:
  New weights
* **__group_865__new_gradients** (optional) - **T3**:
  New gradients
* **__group_865__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_865__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_865__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_866__new_weights** (optional) - **T2**:
  New weights
* **__group_866__new_gradients** (optional) - **T3**:
  New gradients
* **__group_866__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_866__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_866__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_867__new_weights** (optional) - **T2**:
  New weights
* **__group_867__new_gradients** (optional) - **T3**:
  New gradients
* **__group_867__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_867__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_867__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_868__new_weights** (optional) - **T2**:
  New weights
* **__group_868__new_gradients** (optional) - **T3**:
  New gradients
* **__group_868__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_868__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_868__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_869__new_weights** (optional) - **T2**:
  New weights
* **__group_869__new_gradients** (optional) - **T3**:
  New gradients
* **__group_869__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_869__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_869__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_870__new_weights** (optional) - **T2**:
  New weights
* **__group_870__new_gradients** (optional) - **T3**:
  New gradients
* **__group_870__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_870__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_870__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_871__new_weights** (optional) - **T2**:
  New weights
* **__group_871__new_gradients** (optional) - **T3**:
  New gradients
* **__group_871__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_871__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_871__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_872__new_weights** (optional) - **T2**:
  New weights
* **__group_872__new_gradients** (optional) - **T3**:
  New gradients
* **__group_872__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_872__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_872__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_873__new_weights** (optional) - **T2**:
  New weights
* **__group_873__new_gradients** (optional) - **T3**:
  New gradients
* **__group_873__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_873__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_873__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_874__new_weights** (optional) - **T2**:
  New weights
* **__group_874__new_gradients** (optional) - **T3**:
  New gradients
* **__group_874__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_874__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_874__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_875__new_weights** (optional) - **T2**:
  New weights
* **__group_875__new_gradients** (optional) - **T3**:
  New gradients
* **__group_875__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_875__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_875__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_876__new_weights** (optional) - **T2**:
  New weights
* **__group_876__new_gradients** (optional) - **T3**:
  New gradients
* **__group_876__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_876__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_876__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_877__new_weights** (optional) - **T2**:
  New weights
* **__group_877__new_gradients** (optional) - **T3**:
  New gradients
* **__group_877__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_877__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_877__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_878__new_weights** (optional) - **T2**:
  New weights
* **__group_878__new_gradients** (optional) - **T3**:
  New gradients
* **__group_878__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_878__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_878__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_879__new_weights** (optional) - **T2**:
  New weights
* **__group_879__new_gradients** (optional) - **T3**:
  New gradients
* **__group_879__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_879__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_879__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_880__new_weights** (optional) - **T2**:
  New weights
* **__group_880__new_gradients** (optional) - **T3**:
  New gradients
* **__group_880__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_880__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_880__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_881__new_weights** (optional) - **T2**:
  New weights
* **__group_881__new_gradients** (optional) - **T3**:
  New gradients
* **__group_881__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_881__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_881__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_882__new_weights** (optional) - **T2**:
  New weights
* **__group_882__new_gradients** (optional) - **T3**:
  New gradients
* **__group_882__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_882__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_882__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_883__new_weights** (optional) - **T2**:
  New weights
* **__group_883__new_gradients** (optional) - **T3**:
  New gradients
* **__group_883__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_883__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_883__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_884__new_weights** (optional) - **T2**:
  New weights
* **__group_884__new_gradients** (optional) - **T3**:
  New gradients
* **__group_884__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_884__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_884__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_885__new_weights** (optional) - **T2**:
  New weights
* **__group_885__new_gradients** (optional) - **T3**:
  New gradients
* **__group_885__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_885__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_885__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_886__new_weights** (optional) - **T2**:
  New weights
* **__group_886__new_gradients** (optional) - **T3**:
  New gradients
* **__group_886__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_886__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_886__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_887__new_weights** (optional) - **T2**:
  New weights
* **__group_887__new_gradients** (optional) - **T3**:
  New gradients
* **__group_887__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_887__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_887__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_888__new_weights** (optional) - **T2**:
  New weights
* **__group_888__new_gradients** (optional) - **T3**:
  New gradients
* **__group_888__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_888__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_888__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_889__new_weights** (optional) - **T2**:
  New weights
* **__group_889__new_gradients** (optional) - **T3**:
  New gradients
* **__group_889__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_889__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_889__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_890__new_weights** (optional) - **T2**:
  New weights
* **__group_890__new_gradients** (optional) - **T3**:
  New gradients
* **__group_890__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_890__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_890__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_891__new_weights** (optional) - **T2**:
  New weights
* **__group_891__new_gradients** (optional) - **T3**:
  New gradients
* **__group_891__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_891__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_891__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_892__new_weights** (optional) - **T2**:
  New weights
* **__group_892__new_gradients** (optional) - **T3**:
  New gradients
* **__group_892__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_892__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_892__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_893__new_weights** (optional) - **T2**:
  New weights
* **__group_893__new_gradients** (optional) - **T3**:
  New gradients
* **__group_893__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_893__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_893__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_894__new_weights** (optional) - **T2**:
  New weights
* **__group_894__new_gradients** (optional) - **T3**:
  New gradients
* **__group_894__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_894__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_894__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_895__new_weights** (optional) - **T2**:
  New weights
* **__group_895__new_gradients** (optional) - **T3**:
  New gradients
* **__group_895__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_895__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_895__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_896__new_weights** (optional) - **T2**:
  New weights
* **__group_896__new_gradients** (optional) - **T3**:
  New gradients
* **__group_896__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_896__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_896__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_897__new_weights** (optional) - **T2**:
  New weights
* **__group_897__new_gradients** (optional) - **T3**:
  New gradients
* **__group_897__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_897__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_897__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_898__new_weights** (optional) - **T2**:
  New weights
* **__group_898__new_gradients** (optional) - **T3**:
  New gradients
* **__group_898__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_898__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_898__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_899__new_weights** (optional) - **T2**:
  New weights
* **__group_899__new_gradients** (optional) - **T3**:
  New gradients
* **__group_899__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_899__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_899__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_900__new_weights** (optional) - **T2**:
  New weights
* **__group_900__new_gradients** (optional) - **T3**:
  New gradients
* **__group_900__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_900__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_900__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_901__new_weights** (optional) - **T2**:
  New weights
* **__group_901__new_gradients** (optional) - **T3**:
  New gradients
* **__group_901__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_901__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_901__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_902__new_weights** (optional) - **T2**:
  New weights
* **__group_902__new_gradients** (optional) - **T3**:
  New gradients
* **__group_902__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_902__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_902__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_903__new_weights** (optional) - **T2**:
  New weights
* **__group_903__new_gradients** (optional) - **T3**:
  New gradients
* **__group_903__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_903__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_903__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_904__new_weights** (optional) - **T2**:
  New weights
* **__group_904__new_gradients** (optional) - **T3**:
  New gradients
* **__group_904__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_904__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_904__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_905__new_weights** (optional) - **T2**:
  New weights
* **__group_905__new_gradients** (optional) - **T3**:
  New gradients
* **__group_905__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_905__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_905__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_906__new_weights** (optional) - **T2**:
  New weights
* **__group_906__new_gradients** (optional) - **T3**:
  New gradients
* **__group_906__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_906__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_906__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_907__new_weights** (optional) - **T2**:
  New weights
* **__group_907__new_gradients** (optional) - **T3**:
  New gradients
* **__group_907__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_907__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_907__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_908__new_weights** (optional) - **T2**:
  New weights
* **__group_908__new_gradients** (optional) - **T3**:
  New gradients
* **__group_908__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_908__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_908__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_909__new_weights** (optional) - **T2**:
  New weights
* **__group_909__new_gradients** (optional) - **T3**:
  New gradients
* **__group_909__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_909__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_909__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_910__new_weights** (optional) - **T2**:
  New weights
* **__group_910__new_gradients** (optional) - **T3**:
  New gradients
* **__group_910__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_910__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_910__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_911__new_weights** (optional) - **T2**:
  New weights
* **__group_911__new_gradients** (optional) - **T3**:
  New gradients
* **__group_911__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_911__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_911__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_912__new_weights** (optional) - **T2**:
  New weights
* **__group_912__new_gradients** (optional) - **T3**:
  New gradients
* **__group_912__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_912__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_912__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_913__new_weights** (optional) - **T2**:
  New weights
* **__group_913__new_gradients** (optional) - **T3**:
  New gradients
* **__group_913__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_913__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_913__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_914__new_weights** (optional) - **T2**:
  New weights
* **__group_914__new_gradients** (optional) - **T3**:
  New gradients
* **__group_914__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_914__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_914__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_915__new_weights** (optional) - **T2**:
  New weights
* **__group_915__new_gradients** (optional) - **T3**:
  New gradients
* **__group_915__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_915__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_915__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_916__new_weights** (optional) - **T2**:
  New weights
* **__group_916__new_gradients** (optional) - **T3**:
  New gradients
* **__group_916__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_916__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_916__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_917__new_weights** (optional) - **T2**:
  New weights
* **__group_917__new_gradients** (optional) - **T3**:
  New gradients
* **__group_917__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_917__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_917__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_918__new_weights** (optional) - **T2**:
  New weights
* **__group_918__new_gradients** (optional) - **T3**:
  New gradients
* **__group_918__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_918__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_918__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_919__new_weights** (optional) - **T2**:
  New weights
* **__group_919__new_gradients** (optional) - **T3**:
  New gradients
* **__group_919__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_919__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_919__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_920__new_weights** (optional) - **T2**:
  New weights
* **__group_920__new_gradients** (optional) - **T3**:
  New gradients
* **__group_920__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_920__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_920__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_921__new_weights** (optional) - **T2**:
  New weights
* **__group_921__new_gradients** (optional) - **T3**:
  New gradients
* **__group_921__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_921__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_921__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_922__new_weights** (optional) - **T2**:
  New weights
* **__group_922__new_gradients** (optional) - **T3**:
  New gradients
* **__group_922__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_922__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_922__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_923__new_weights** (optional) - **T2**:
  New weights
* **__group_923__new_gradients** (optional) - **T3**:
  New gradients
* **__group_923__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_923__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_923__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_924__new_weights** (optional) - **T2**:
  New weights
* **__group_924__new_gradients** (optional) - **T3**:
  New gradients
* **__group_924__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_924__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_924__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_925__new_weights** (optional) - **T2**:
  New weights
* **__group_925__new_gradients** (optional) - **T3**:
  New gradients
* **__group_925__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_925__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_925__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_926__new_weights** (optional) - **T2**:
  New weights
* **__group_926__new_gradients** (optional) - **T3**:
  New gradients
* **__group_926__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_926__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_926__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_927__new_weights** (optional) - **T2**:
  New weights
* **__group_927__new_gradients** (optional) - **T3**:
  New gradients
* **__group_927__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_927__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_927__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_928__new_weights** (optional) - **T2**:
  New weights
* **__group_928__new_gradients** (optional) - **T3**:
  New gradients
* **__group_928__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_928__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_928__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_929__new_weights** (optional) - **T2**:
  New weights
* **__group_929__new_gradients** (optional) - **T3**:
  New gradients
* **__group_929__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_929__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_929__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_930__new_weights** (optional) - **T2**:
  New weights
* **__group_930__new_gradients** (optional) - **T3**:
  New gradients
* **__group_930__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_930__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_930__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_931__new_weights** (optional) - **T2**:
  New weights
* **__group_931__new_gradients** (optional) - **T3**:
  New gradients
* **__group_931__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_931__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_931__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_932__new_weights** (optional) - **T2**:
  New weights
* **__group_932__new_gradients** (optional) - **T3**:
  New gradients
* **__group_932__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_932__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_932__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_933__new_weights** (optional) - **T2**:
  New weights
* **__group_933__new_gradients** (optional) - **T3**:
  New gradients
* **__group_933__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_933__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_933__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_934__new_weights** (optional) - **T2**:
  New weights
* **__group_934__new_gradients** (optional) - **T3**:
  New gradients
* **__group_934__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_934__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_934__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_935__new_weights** (optional) - **T2**:
  New weights
* **__group_935__new_gradients** (optional) - **T3**:
  New gradients
* **__group_935__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_935__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_935__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_936__new_weights** (optional) - **T2**:
  New weights
* **__group_936__new_gradients** (optional) - **T3**:
  New gradients
* **__group_936__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_936__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_936__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_937__new_weights** (optional) - **T2**:
  New weights
* **__group_937__new_gradients** (optional) - **T3**:
  New gradients
* **__group_937__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_937__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_937__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_938__new_weights** (optional) - **T2**:
  New weights
* **__group_938__new_gradients** (optional) - **T3**:
  New gradients
* **__group_938__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_938__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_938__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_939__new_weights** (optional) - **T2**:
  New weights
* **__group_939__new_gradients** (optional) - **T3**:
  New gradients
* **__group_939__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_939__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_939__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_940__new_weights** (optional) - **T2**:
  New weights
* **__group_940__new_gradients** (optional) - **T3**:
  New gradients
* **__group_940__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_940__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_940__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_941__new_weights** (optional) - **T2**:
  New weights
* **__group_941__new_gradients** (optional) - **T3**:
  New gradients
* **__group_941__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_941__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_941__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_942__new_weights** (optional) - **T2**:
  New weights
* **__group_942__new_gradients** (optional) - **T3**:
  New gradients
* **__group_942__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_942__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_942__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_943__new_weights** (optional) - **T2**:
  New weights
* **__group_943__new_gradients** (optional) - **T3**:
  New gradients
* **__group_943__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_943__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_943__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_944__new_weights** (optional) - **T2**:
  New weights
* **__group_944__new_gradients** (optional) - **T3**:
  New gradients
* **__group_944__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_944__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_944__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_945__new_weights** (optional) - **T2**:
  New weights
* **__group_945__new_gradients** (optional) - **T3**:
  New gradients
* **__group_945__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_945__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_945__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_946__new_weights** (optional) - **T2**:
  New weights
* **__group_946__new_gradients** (optional) - **T3**:
  New gradients
* **__group_946__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_946__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_946__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_947__new_weights** (optional) - **T2**:
  New weights
* **__group_947__new_gradients** (optional) - **T3**:
  New gradients
* **__group_947__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_947__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_947__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_948__new_weights** (optional) - **T2**:
  New weights
* **__group_948__new_gradients** (optional) - **T3**:
  New gradients
* **__group_948__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_948__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_948__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_949__new_weights** (optional) - **T2**:
  New weights
* **__group_949__new_gradients** (optional) - **T3**:
  New gradients
* **__group_949__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_949__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_949__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_950__new_weights** (optional) - **T2**:
  New weights
* **__group_950__new_gradients** (optional) - **T3**:
  New gradients
* **__group_950__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_950__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_950__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_951__new_weights** (optional) - **T2**:
  New weights
* **__group_951__new_gradients** (optional) - **T3**:
  New gradients
* **__group_951__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_951__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_951__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_952__new_weights** (optional) - **T2**:
  New weights
* **__group_952__new_gradients** (optional) - **T3**:
  New gradients
* **__group_952__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_952__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_952__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_953__new_weights** (optional) - **T2**:
  New weights
* **__group_953__new_gradients** (optional) - **T3**:
  New gradients
* **__group_953__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_953__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_953__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_954__new_weights** (optional) - **T2**:
  New weights
* **__group_954__new_gradients** (optional) - **T3**:
  New gradients
* **__group_954__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_954__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_954__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_955__new_weights** (optional) - **T2**:
  New weights
* **__group_955__new_gradients** (optional) - **T3**:
  New gradients
* **__group_955__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_955__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_955__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_956__new_weights** (optional) - **T2**:
  New weights
* **__group_956__new_gradients** (optional) - **T3**:
  New gradients
* **__group_956__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_956__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_956__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_957__new_weights** (optional) - **T2**:
  New weights
* **__group_957__new_gradients** (optional) - **T3**:
  New gradients
* **__group_957__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_957__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_957__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_958__new_weights** (optional) - **T2**:
  New weights
* **__group_958__new_gradients** (optional) - **T3**:
  New gradients
* **__group_958__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_958__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_958__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_959__new_weights** (optional) - **T2**:
  New weights
* **__group_959__new_gradients** (optional) - **T3**:
  New gradients
* **__group_959__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_959__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_959__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_960__new_weights** (optional) - **T2**:
  New weights
* **__group_960__new_gradients** (optional) - **T3**:
  New gradients
* **__group_960__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_960__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_960__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_961__new_weights** (optional) - **T2**:
  New weights
* **__group_961__new_gradients** (optional) - **T3**:
  New gradients
* **__group_961__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_961__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_961__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_962__new_weights** (optional) - **T2**:
  New weights
* **__group_962__new_gradients** (optional) - **T3**:
  New gradients
* **__group_962__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_962__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_962__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_963__new_weights** (optional) - **T2**:
  New weights
* **__group_963__new_gradients** (optional) - **T3**:
  New gradients
* **__group_963__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_963__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_963__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_964__new_weights** (optional) - **T2**:
  New weights
* **__group_964__new_gradients** (optional) - **T3**:
  New gradients
* **__group_964__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_964__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_964__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_965__new_weights** (optional) - **T2**:
  New weights
* **__group_965__new_gradients** (optional) - **T3**:
  New gradients
* **__group_965__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_965__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_965__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_966__new_weights** (optional) - **T2**:
  New weights
* **__group_966__new_gradients** (optional) - **T3**:
  New gradients
* **__group_966__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_966__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_966__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_967__new_weights** (optional) - **T2**:
  New weights
* **__group_967__new_gradients** (optional) - **T3**:
  New gradients
* **__group_967__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_967__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_967__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_968__new_weights** (optional) - **T2**:
  New weights
* **__group_968__new_gradients** (optional) - **T3**:
  New gradients
* **__group_968__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_968__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_968__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_969__new_weights** (optional) - **T2**:
  New weights
* **__group_969__new_gradients** (optional) - **T3**:
  New gradients
* **__group_969__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_969__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_969__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_970__new_weights** (optional) - **T2**:
  New weights
* **__group_970__new_gradients** (optional) - **T3**:
  New gradients
* **__group_970__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_970__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_970__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_971__new_weights** (optional) - **T2**:
  New weights
* **__group_971__new_gradients** (optional) - **T3**:
  New gradients
* **__group_971__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_971__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_971__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_972__new_weights** (optional) - **T2**:
  New weights
* **__group_972__new_gradients** (optional) - **T3**:
  New gradients
* **__group_972__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_972__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_972__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_973__new_weights** (optional) - **T2**:
  New weights
* **__group_973__new_gradients** (optional) - **T3**:
  New gradients
* **__group_973__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_973__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_973__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_974__new_weights** (optional) - **T2**:
  New weights
* **__group_974__new_gradients** (optional) - **T3**:
  New gradients
* **__group_974__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_974__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_974__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_975__new_weights** (optional) - **T2**:
  New weights
* **__group_975__new_gradients** (optional) - **T3**:
  New gradients
* **__group_975__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_975__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_975__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_976__new_weights** (optional) - **T2**:
  New weights
* **__group_976__new_gradients** (optional) - **T3**:
  New gradients
* **__group_976__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_976__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_976__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_977__new_weights** (optional) - **T2**:
  New weights
* **__group_977__new_gradients** (optional) - **T3**:
  New gradients
* **__group_977__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_977__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_977__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_978__new_weights** (optional) - **T2**:
  New weights
* **__group_978__new_gradients** (optional) - **T3**:
  New gradients
* **__group_978__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_978__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_978__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_979__new_weights** (optional) - **T2**:
  New weights
* **__group_979__new_gradients** (optional) - **T3**:
  New gradients
* **__group_979__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_979__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_979__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_980__new_weights** (optional) - **T2**:
  New weights
* **__group_980__new_gradients** (optional) - **T3**:
  New gradients
* **__group_980__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_980__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_980__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_981__new_weights** (optional) - **T2**:
  New weights
* **__group_981__new_gradients** (optional) - **T3**:
  New gradients
* **__group_981__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_981__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_981__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_982__new_weights** (optional) - **T2**:
  New weights
* **__group_982__new_gradients** (optional) - **T3**:
  New gradients
* **__group_982__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_982__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_982__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_983__new_weights** (optional) - **T2**:
  New weights
* **__group_983__new_gradients** (optional) - **T3**:
  New gradients
* **__group_983__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_983__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_983__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_984__new_weights** (optional) - **T2**:
  New weights
* **__group_984__new_gradients** (optional) - **T3**:
  New gradients
* **__group_984__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_984__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_984__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_985__new_weights** (optional) - **T2**:
  New weights
* **__group_985__new_gradients** (optional) - **T3**:
  New gradients
* **__group_985__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_985__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_985__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_986__new_weights** (optional) - **T2**:
  New weights
* **__group_986__new_gradients** (optional) - **T3**:
  New gradients
* **__group_986__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_986__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_986__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_987__new_weights** (optional) - **T2**:
  New weights
* **__group_987__new_gradients** (optional) - **T3**:
  New gradients
* **__group_987__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_987__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_987__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_988__new_weights** (optional) - **T2**:
  New weights
* **__group_988__new_gradients** (optional) - **T3**:
  New gradients
* **__group_988__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_988__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_988__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_989__new_weights** (optional) - **T2**:
  New weights
* **__group_989__new_gradients** (optional) - **T3**:
  New gradients
* **__group_989__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_989__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_989__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_990__new_weights** (optional) - **T2**:
  New weights
* **__group_990__new_gradients** (optional) - **T3**:
  New gradients
* **__group_990__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_990__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_990__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_991__new_weights** (optional) - **T2**:
  New weights
* **__group_991__new_gradients** (optional) - **T3**:
  New gradients
* **__group_991__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_991__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_991__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_992__new_weights** (optional) - **T2**:
  New weights
* **__group_992__new_gradients** (optional) - **T3**:
  New gradients
* **__group_992__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_992__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_992__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_993__new_weights** (optional) - **T2**:
  New weights
* **__group_993__new_gradients** (optional) - **T3**:
  New gradients
* **__group_993__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_993__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_993__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_994__new_weights** (optional) - **T2**:
  New weights
* **__group_994__new_gradients** (optional) - **T3**:
  New gradients
* **__group_994__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_994__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_994__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_995__new_weights** (optional) - **T2**:
  New weights
* **__group_995__new_gradients** (optional) - **T3**:
  New gradients
* **__group_995__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_995__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_995__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_996__new_weights** (optional) - **T2**:
  New weights
* **__group_996__new_gradients** (optional) - **T3**:
  New gradients
* **__group_996__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_996__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_996__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_997__new_weights** (optional) - **T2**:
  New weights
* **__group_997__new_gradients** (optional) - **T3**:
  New gradients
* **__group_997__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_997__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_997__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_998__new_weights** (optional) - **T2**:
  New weights
* **__group_998__new_gradients** (optional) - **T3**:
  New gradients
* **__group_998__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_998__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_998__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_999__new_weights** (optional) - **T2**:
  New weights
* **__group_999__new_gradients** (optional) - **T3**:
  New gradients
* **__group_999__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_999__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_999__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1000__new_weights** (optional) - **T2**:
  New weights
* **__group_1000__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1000__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1000__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1000__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1001__new_weights** (optional) - **T2**:
  New weights
* **__group_1001__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1001__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1001__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1001__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1002__new_weights** (optional) - **T2**:
  New weights
* **__group_1002__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1002__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1002__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1002__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1003__new_weights** (optional) - **T2**:
  New weights
* **__group_1003__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1003__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1003__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1003__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1004__new_weights** (optional) - **T2**:
  New weights
* **__group_1004__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1004__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1004__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1004__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1005__new_weights** (optional) - **T2**:
  New weights
* **__group_1005__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1005__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1005__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1005__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1006__new_weights** (optional) - **T2**:
  New weights
* **__group_1006__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1006__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1006__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1006__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1007__new_weights** (optional) - **T2**:
  New weights
* **__group_1007__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1007__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1007__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1007__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1008__new_weights** (optional) - **T2**:
  New weights
* **__group_1008__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1008__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1008__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1008__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1009__new_weights** (optional) - **T2**:
  New weights
* **__group_1009__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1009__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1009__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1009__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1010__new_weights** (optional) - **T2**:
  New weights
* **__group_1010__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1010__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1010__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1010__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1011__new_weights** (optional) - **T2**:
  New weights
* **__group_1011__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1011__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1011__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1011__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1012__new_weights** (optional) - **T2**:
  New weights
* **__group_1012__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1012__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1012__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1012__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1013__new_weights** (optional) - **T2**:
  New weights
* **__group_1013__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1013__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1013__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1013__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1014__new_weights** (optional) - **T2**:
  New weights
* **__group_1014__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1014__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1014__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1014__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1015__new_weights** (optional) - **T2**:
  New weights
* **__group_1015__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1015__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1015__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1015__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1016__new_weights** (optional) - **T2**:
  New weights
* **__group_1016__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1016__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1016__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1016__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1017__new_weights** (optional) - **T2**:
  New weights
* **__group_1017__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1017__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1017__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1017__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1018__new_weights** (optional) - **T2**:
  New weights
* **__group_1018__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1018__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1018__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1018__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1019__new_weights** (optional) - **T2**:
  New weights
* **__group_1019__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1019__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1019__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1019__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1020__new_weights** (optional) - **T2**:
  New weights
* **__group_1020__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1020__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1020__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1020__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1021__new_weights** (optional) - **T2**:
  New weights
* **__group_1021__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1021__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1021__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1021__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1022__new_weights** (optional) - **T2**:
  New weights
* **__group_1022__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1022__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1022__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1022__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights
* **__group_1023__new_weights** (optional) - **T2**:
  New weights
* **__group_1023__new_gradients** (optional) - **T3**:
  New gradients
* **__group_1023__new_moment_1** (optional) - **T4**:
  New averaged gradients
* **__group_1023__new_moment_2** (optional) - **T4**:
  New averaged squared gradients
* **__group_1023__new_mixed_precision_weights** (optional) - **T_MIXED_PRECISION_FP**:
  New FP16 or BF16 weights

**Examples**
