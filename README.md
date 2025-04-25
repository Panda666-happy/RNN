# RNN

# 1 两个模型的核心差异体现在什么机制上？B
## A. 字符编码方式不同
## B. 是否考虑国家信息作为生成条件
## C. RNN单元类型不同（GRU/LSTM）
## D. 损失函数计算方式不同

# 2 在条件生成模型（Model2_Conditioned_Surname_Generation）中，国家信息通过什么方式影响生成过程？ B
## A. 作为额外的输入特征拼接
## B. 作为GRU的初始隐藏状态
## C. 作为注意力机制的key
## D. 作为输出层的偏置项

# 3 文件2中新增的nation_emb层的主要作用是： B
# self.nation_emb = nn.Embedding(num_nationalities, rnn_hidden_size)
## A. 将字符索引映射为稠密向量
## B. 将国家标签转换为隐藏状态初始化向量
## C. 生成姓氏的长度控制参数
## D. 计算交叉熵损失的辅助参数

# 4 对比两个文件的sample_from_model函数，文件2新增了哪个关键参数？ B
## A. temperature
## B. nationalities
## C. device
## D. max_length

# 数据预处理验证
![屏幕截图 2025-04-25 095537](https://github.com/user-attachments/assets/cfa60532-fff7-477f-9474-6ff8f94ec6db)
# 模型结构验证
![屏幕截图 2025-04-25 094443](https://github.com/user-attachments/assets/2d9f5abb-28ce-4cae-bae1-1a87ad3c0997)
# RNN处理验证
![屏幕截图 2025-04-25 094502](https://github.com/user-attachments/assets/c6ee25db-863d-42ee-b75f-f7b003536930)
# 损失值
![屏幕截图 2025-04-25 095242](https://github.com/user-attachments/assets/6070dade-a637-47d0-ae40-9126c866ae2f)
# 结果
![屏幕截图 2025-04-25 095319](https://github.com/user-attachments/assets/f303510c-1c18-49bb-9457-bfe72fc741d2)

![屏幕截图 2025-04-22 185102](https://github.com/user-attachments/assets/ae6e5bb2-5e0d-4ac5-9f70-6b75941e5a72)

![屏幕截图 2025-04-22 192857](https://github.com/user-attachments/assets/9a29d70e-61eb-4579-b736-cf773bba3d3a)

![屏幕截图 2025-04-22 191724](https://github.com/user-attachments/assets/ec38b7d6-3d20-4216-8f6e-c902c5753e92)
