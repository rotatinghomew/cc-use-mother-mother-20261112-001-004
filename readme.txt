测试：python3 -m unittest discover -s tests/rights_cases -p 'test_*.py'
构建：python3 -m compileall -q design_rights_chain tests/rights_cases
验收：python3 -m design_rights_chain.casework.command fixtures/demo.json --database /tmp/design_rights_chain-acceptance.sqlite3
所有输入均为本地合成数据，运行不需要网络。
