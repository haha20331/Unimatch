# Unimatch
由vscode 連接到140.123.104.128(7*1080ti) or 140.123.104.126(2*A40)
進環境 conda activate unimatch
進入資料夾~/UniMatch

在/home/yea0826/UniMatch/splits/Med中有許多不同組合的data分割方式
要把要用的分割方式的檔名更名為”home/yea0826/UniMatch/splits/Med/6”

在/home/yea0826/UniMatch/scripts/train.sh中第17行更改結果儲存路徑
train.sh中也可更改dataset, method, exp (resnet50 or 101), split

在/home/yea0826/UniMatch/supervised.py中第86~89行更改IoU & Dice score log儲存路徑和名稱

執行sh scripts/train.sh 2 12345  (2是gpu數，12345是port number，隨便設?)
