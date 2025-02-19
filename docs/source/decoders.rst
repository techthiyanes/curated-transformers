Decoders
========

Architectures
-------------

These modules represent the supported decoder-only architectures.

.. autoclass:: curated_transformers.models.module.DecoderModule
   :members:
   :show-inheritance:

.. autoclass:: curated_transformers.models.GPTNeoXDecoder
   :members:
   :show-inheritance:

.. autoclass:: curated_transformers.models.LLaMADecoder
   :members:
   :show-inheritance:

.. autoclass:: curated_transformers.models.FalconDecoder
   :members:
   :show-inheritance:


Downloading
-----------

Each decoder type provides a ``from_hf_hub`` function that will load a model
from Hugging Face Hub. If you want to load a decoder without committing to a 
specific decoder type, you can use the :class:`~.auto_model.AutoDecoder`
class. This class also provides a ``from_hf_hub`` method but will try to infer 
the correct type automatically.

.. autoclass:: curated_transformers.models.auto_model.AutoDecoder
   :members:


.. _decoder config:

Model Configuration
-------------------

GPT-NeoX
^^^^^^^^

.. autoclass:: curated_transformers.models.gpt_neox.config.GPTNeoXConfig
   :members:

.. autoclass:: curated_transformers.models.gpt_neox.config.GPTNeoXLayerConfig
   :members:

.. autoclass:: curated_transformers.models.gpt_neox.config.GPTNeoXEmbeddingConfig
   :members:

.. autoclass:: curated_transformers.models.gpt_neox.config.GPTNeoXAttentionConfig
   :members:

LLaMA
^^^^^

.. autoclass:: curated_transformers.models.llama.config.LLaMAConfig
   :members:

.. autoclass:: curated_transformers.models.llama.config.LLaMALayerConfig
   :members:

.. autoclass:: curated_transformers.models.llama.config.LLaMAEmbeddingConfig
   :members:

.. autoclass:: curated_transformers.models.llama.config.LLaMAAttentionConfig
   :members:

Falcon
^^^^^^

.. autoclass:: curated_transformers.models.falcon.config.FalconConfig
   :members:

.. autoclass:: curated_transformers.models.falcon.config.FalconLayerConfig
   :members:

.. autoclass:: curated_transformers.models.falcon.config.FalconEmbeddingConfig
   :members:

.. autoclass:: curated_transformers.models.falcon.config.FalconAttentionConfig
   :members: