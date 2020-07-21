# ******************************************************************************
# Copyright 2019-2020 Intel Corporation
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
# ******************************************************************************

# Installation

```bash
python3.6 -m pip install -U pip setuptools virtualenv
python3.6 -m venv my_env
source my_env/bin/activate
git clone https://github.com/NervanaSystems/nlp-architect.git
pip install -e nlp-architect

git clone https://github.com/huggingface/transformers
cd transformers
pip install .
pip install -r ./examples/requirements.txt

pip install -U git+http://github.com/PyTorchLightning/pytorch-lightning/

python3 preprocess.py train.txt.tmp > train.txt
python3 preprocess.py dev.txt.tmp > dev.txt
python3 preprocess.py test.txt.tmp > test.txt

```