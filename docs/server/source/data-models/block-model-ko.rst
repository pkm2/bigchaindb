
.. Copyright BigchainDB GmbH and BigchainDB contributors
   SPDX-License-Identifier: (Apache-2.0 AND CC-BY-4.0)
   Code is Apache-2.0 and docs are CC-BY-4.0

.. _the-block-model:

블록 모델
===============

블록은 이 페이지에서 설명한대로 특정 스키마가 있는 JSON 객체입니다. 
블록에는 다음 JSON 키 (이름 또는 필드라고도 함)가 있어야 합니다.

.. code-block:: json

    {
      "height": "<Height of the block>",
      "transactions": ["<List of transactions>"]
    }


블록의 JSON 키
------------------------

**높이**

블록 ``"height"`` (``integer``) 은 주어진 블록이 커밋되었을 때 블록 체인의 높이를 나타냅니다.
블록 체인 높이가 단조롭게 증가하기 때문에 블록 높이는 ID로 간주 될 수 있습니다.

**비고**: 최초의 블록 height은 ``0``


**트랜잭션**

블록에 포함 된 트랜잭션의 목록 :ref:`트랜잭션 <the-transaction-model>` 
(각 트랜잭션은 JSON 객체입니다.)
