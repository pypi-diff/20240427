# Comparing `tmp/mser-0.0.1-py3-none-any.whl.zip` & `tmp/mser-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 36175 bytes, number of entries: 24
--rw-rw-rw-  2.0 fat       87 b- defN 23-Aug-17 08:48 mser/__init__.py
--rw-rw-rw-  2.0 fat     7834 b- defN 23-Aug-18 11:24 mser/predict.py
--rw-rw-rw-  2.0 fat    27201 b- defN 23-Aug-18 11:14 mser/trainer.py
+Zip file size: 39555 bytes, number of entries: 24
+-rw-rw-rw-  2.0 fat       89 b- defN 24-Apr-27 05:49 mser/__init__.py
+-rw-rw-rw-  2.0 fat     8006 b- defN 24-Apr-08 14:49 mser/predict.py
+-rw-rw-rw-  2.0 fat    30475 b- defN 24-Apr-27 04:46 mser/trainer.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-30 13:17 mser/data_utils/__init__.py
--rw-rw-rw-  2.0 fat    22286 b- defN 23-Aug-13 08:17 mser/data_utils/audio.py
+-rw-rw-rw-  2.0 fat    22217 b- defN 24-Apr-27 05:31 mser/data_utils/audio.py
 -rw-rw-rw-  2.0 fat      965 b- defN 23-Feb-15 12:59 mser/data_utils/collate_fn.py
--rw-rw-rw-  2.0 fat     3335 b- defN 23-Aug-17 14:45 mser/data_utils/featurizer.py
--rw-rw-rw-  2.0 fat     6625 b- defN 23-Aug-18 10:57 mser/data_utils/reader.py
--rw-rw-rw-  2.0 fat     1572 b- defN 23-Aug-07 14:52 mser/data_utils/spec_aug.py
+-rw-rw-rw-  2.0 fat     4696 b- defN 24-Apr-08 14:49 mser/data_utils/featurizer.py
+-rw-rw-rw-  2.0 fat     6712 b- defN 24-Apr-08 14:49 mser/data_utils/reader.py
 -rw-rw-rw-  2.0 fat     5652 b- defN 23-Mar-28 12:05 mser/data_utils/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-16 05:03 mser/metric/__init__.py
 -rw-rw-rw-  2.0 fat      329 b- defN 23-Aug-07 15:15 mser/metric/metrics.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-30 13:17 mser/models/__init__.py
--rw-rw-rw-  2.0 fat      854 b- defN 23-Aug-17 16:00 mser/models/bidirectional_lstm.py
+-rw-rw-rw-  2.0 fat      420 b- defN 24-Apr-08 14:49 mser/models/base_model.py
+-rw-rw-rw-  2.0 fat      845 b- defN 24-Apr-08 14:49 mser/models/bi_lstm.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-30 13:17 mser/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2839 b- defN 23-Jan-30 13:17 mser/utils/logger.py
 -rw-rw-rw-  2.0 fat     1067 b- defN 23-Mar-23 11:45 mser/utils/record.py
 -rw-rw-rw-  2.0 fat     1496 b- defN 23-Aug-06 15:19 mser/utils/scheduler.py
--rw-rw-rw-  2.0 fat     3363 b- defN 23-Aug-13 08:17 mser/utils/utils.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Aug-18 11:27 mser-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11302 b- defN 23-Aug-18 11:27 mser-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-18 11:27 mser-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Aug-18 11:27 mser-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1876 b- defN 23-Aug-18 11:27 mser-0.0.1.dist-info/RECORD
-24 files, 110338 bytes uncompressed, 33169 bytes compressed:  69.9%
+-rw-rw-rw-  2.0 fat     4299 b- defN 24-Apr-27 04:49 mser/utils/utils.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-27 05:50 mser-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    18150 b- defN 24-Apr-27 05:50 mser-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-27 05:50 mser-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-27 05:50 mser-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1862 b- defN 24-Apr-27 05:50 mser-0.0.3.dist-info/RECORD
+24 files, 121774 bytes uncompressed, 36575 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -18,30 +18,30 @@
 
 Filename: mser/data_utils/featurizer.py
 Comment: 
 
 Filename: mser/data_utils/reader.py
 Comment: 
 
-Filename: mser/data_utils/spec_aug.py
-Comment: 
-
 Filename: mser/data_utils/utils.py
 Comment: 
 
 Filename: mser/metric/__init__.py
 Comment: 
 
 Filename: mser/metric/metrics.py
 Comment: 
 
 Filename: mser/models/__init__.py
 Comment: 
 
-Filename: mser/models/bidirectional_lstm.py
+Filename: mser/models/base_model.py
+Comment: 
+
+Filename: mser/models/bi_lstm.py
 Comment: 
 
 Filename: mser/utils/__init__.py
 Comment: 
 
 Filename: mser/utils/logger.py
 Comment: 
@@ -51,23 +51,23 @@
 
 Filename: mser/utils/scheduler.py
 Comment: 
 
 Filename: mser/utils/utils.py
 Comment: 
 
-Filename: mser-0.0.1.dist-info/LICENSE
+Filename: mser-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: mser-0.0.1.dist-info/METADATA
+Filename: mser-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: mser-0.0.1.dist-info/WHEEL
+Filename: mser-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: mser-0.0.1.dist-info/top_level.txt
+Filename: mser-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: mser-0.0.1.dist-info/RECORD
+Filename: mser-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mser/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "0.0.1"
+__version__ = "0.0.3"
 # 项目支持的模型
-SUPPORT_MODEL = ['BidirectionalLSTM']
+SUPPORT_MODEL = ['BiLSTM', 'BaseModel']
```

## mser/predict.py

```diff
@@ -6,25 +6,26 @@
 import numpy as np
 import torch
 import yaml
 
 from mser import SUPPORT_MODEL
 from mser.data_utils.audio import AudioSegment
 from mser.data_utils.featurizer import AudioFeaturizer
-from mser.models.bidirectional_lstm import BidirectionalLSTM
+from mser.models.bi_lstm import BiLSTM
+from mser.models.base_model import BaseModel
 from mser.utils.logger import setup_logger
 from mser.utils.utils import dict_to_object, print_arguments
 
 logger = setup_logger(__name__)
 
 
 class MSERPredictor:
     def __init__(self,
                  configs,
-                 model_path='models/EcapaTdnn_Fbank/best_model/',
+                 model_path='models/BiLSTM_Emotion2Vec/best_model/',
                  use_gpu=True):
         """
         声音分类预测工具
         :param configs: 配置参数
         :param model_path: 导出的预测模型文件夹路径
         :param use_gpu: 是否使用GPU预测
         """
@@ -48,16 +49,18 @@
         with open(self.configs.dataset_conf.label_list_path, 'r', encoding='utf-8') as f:
             lines = f.readlines()
         self.class_labels = [l.replace('\n', '') for l in lines]
         # 自动获取列表数量
         if self.configs.model_conf.num_class is None:
             self.configs.model_conf.num_class = len(self.class_labels)
         # 获取模型
-        if self.configs.use_model == 'BidirectionalLSTM':
-            self.predictor = BidirectionalLSTM(input_size=self._audio_featurizer.feature_dim, **self.configs.model_conf)
+        if self.configs.use_model == 'BiLSTM':
+            self.predictor = BiLSTM(input_size=self._audio_featurizer.feature_dim, **self.configs.model_conf)
+        elif self.configs.use_model == 'BaseModel':
+            self.predictor = BaseModel(input_size=self._audio_featurizer.feature_dim, **self.configs.model_conf)
         else:
             raise Exception(f'{self.configs.use_model} 模型不存在！')
         self.predictor.to(self.device)
         # 加载模型
         if os.path.isdir(model_path):
             model_path = os.path.join(model_path, 'model.pth')
         assert os.path.exists(model_path), f"{model_path} 模型不存在！"
```

## mser/trainer.py

```diff
@@ -19,17 +19,17 @@
 from tqdm import tqdm
 from visualdl import LogWriter
 
 from mser import SUPPORT_MODEL, __version__
 from mser.data_utils.collate_fn import collate_fn
 from mser.data_utils.featurizer import AudioFeaturizer
 from mser.data_utils.reader import CustomDataset
-from mser.data_utils.spec_aug import SpecAug
 from mser.metric.metrics import accuracy
-from mser.models.bidirectional_lstm import BidirectionalLSTM
+from mser.models.base_model import BaseModel
+from mser.models.bi_lstm import BiLSTM
 from mser.utils.logger import setup_logger
 from mser.utils.scheduler import WarmupCosineSchedulerLR
 from mser.utils.utils import dict_to_object, plot_confusion_matrix, print_arguments
 
 logger = setup_logger(__name__)
 
 
@@ -59,22 +59,24 @@
         self.amp_scaler = None
         # 获取分类标签
         with open(self.configs.dataset_conf.label_list_path, 'r', encoding='utf-8') as f:
             lines = f.readlines()
         self.class_labels = [l.replace('\n', '') for l in lines]
         if platform.system().lower() == 'windows':
             self.configs.dataset_conf.dataLoader.num_workers = 0
-            logger.warning('Windows系统不支持多线程读取数据，已自动关闭！')
-        # 特征增强
-        self.spec_aug = SpecAug(**self.configs.dataset_conf.get('spec_aug_args', {}))
-        self.spec_aug.to(self.device)
-        # 获取分类标签
-        with open(self.configs.dataset_conf.label_list_path, 'r', encoding='utf-8') as f:
-            lines = f.readlines()
-        self.class_labels = [l.replace('\n', '') for l in lines]
+            logger.warning('Windows系统不支持多线程读取数据，已自动使用单线程读取！')
+        if self.configs.preprocess_conf.feature_method == 'Emotion2Vec':
+            self.configs.dataset_conf.dataLoader.num_workers = 0
+            logger.warning('Emotion2Vec特征提取方法不支持多线程，已自动使用单线程提取特征！')
+        self.max_step, self.train_step = None, None
+        self.train_loss, self.train_acc = None, None
+        self.train_eta_sec = None
+        self.eval_loss, self.eval_acc = None, None
+        self.test_log_step, self.train_log_step = 0, 0
+        self.stop_train, self.stop_eval = False, False
 
     def __setup_dataloader(self, is_train=False):
         self.audio_featurizer = AudioFeaturizer(feature_method=self.configs.preprocess_conf.feature_method,
                                                 method_args=self.configs.preprocess_conf.get('method_args', {}))
         if is_train:
             self.train_dataset = CustomDataset(data_list_path=self.configs.dataset_conf.train_list,
                                                audio_featurizer=self.audio_featurizer,
@@ -114,69 +116,98 @@
                                       num_workers=self.configs.dataset_conf.dataLoader.num_workers)
 
     # 获取用于归一化的文件
     def get_standard_file(self):
         audio_featurizer = AudioFeaturizer(feature_method=self.configs.preprocess_conf.feature_method,
                                            method_args=self.configs.preprocess_conf.get('method_args', {}))
         # 获取测试数据
-        test_dataset = CustomDataset(data_list_path=self.configs.dataset_conf.test_list,
+        test_dataset = CustomDataset(data_list_path=self.configs.dataset_conf.train_list,
                                      audio_featurizer=audio_featurizer,
-                                     scaler_path=self.configs.dataset_conf.scaler_path,
                                      do_vad=self.configs.dataset_conf.do_vad,
-                                     max_duration=self.configs.dataset_conf.eval_conf.max_duration,
+                                     max_duration=self.configs.dataset_conf.max_duration,
                                      min_duration=self.configs.dataset_conf.min_duration,
                                      sample_rate=self.configs.dataset_conf.sample_rate,
                                      use_dB_normalization=self.configs.dataset_conf.use_dB_normalization,
                                      target_dB=self.configs.dataset_conf.target_dB,
                                      mode='create_data')
         data = []
         for i in tqdm(range(len(test_dataset))):
             feature, _ = test_dataset[i]
-
             data.append(feature)
         scaler = StandardScaler().fit(data)
         joblib.dump(scaler, self.configs.dataset_conf.scaler_path)
         logger.info(f'归一化文件保存在：{self.configs.dataset_conf.scaler_path}')
 
+    # 提取特征保存文件
+    def extract_features(self, save_dir='dataset/features'):
+        os.makedirs(save_dir, exist_ok=True)
+        audio_featurizer = AudioFeaturizer(feature_method=self.configs.preprocess_conf.feature_method,
+                                           method_args=self.configs.preprocess_conf.get('method_args', {}))
+        for i, data_list in enumerate([self.configs.dataset_conf.train_list, self.configs.dataset_conf.test_list]):
+            max_duration = self.configs.dataset_conf.max_duration if i == 0 else self.configs.dataset_conf.eval_conf.max_duration
+            # 获取测试数据
+            test_dataset = CustomDataset(data_list_path=data_list,
+                                         audio_featurizer=audio_featurizer,
+                                         do_vad=self.configs.dataset_conf.do_vad,
+                                         max_duration=max_duration,
+                                         min_duration=self.configs.dataset_conf.min_duration,
+                                         sample_rate=self.configs.dataset_conf.sample_rate,
+                                         use_dB_normalization=self.configs.dataset_conf.use_dB_normalization,
+                                         target_dB=self.configs.dataset_conf.target_dB,
+                                         mode='create_data')
+            save_data_list = data_list.replace('.txt', '_features.txt')
+            with open(save_data_list, 'w', encoding='utf-8') as f:
+                for i in tqdm(range(len(test_dataset))):
+                    feature, label = test_dataset[i]
+                    label = int(label)
+                    save_path = os.path.join(save_dir, f'{int(time.time() * 1000)}.npy')
+                    np.save(save_path, feature)
+                    f.write(f'{save_path}\t{label}\n')
+            logger.info(f'{data_list}列表中的数据已提取特征完成，新列表为：{save_data_list}')
+
     # 获取模型
     def __setup_model(self, input_size, is_train=False):
         # 自动获取列表数量
         if self.configs.model_conf.num_class is None:
             self.configs.model_conf.num_class = len(self.class_labels)
         # 获取模型
-        if self.configs.use_model == 'BidirectionalLSTM':
-            self.model = BidirectionalLSTM(input_size=input_size, **self.configs.model_conf)
+        if self.configs.use_model == 'BiLSTM':
+            self.model = BiLSTM(input_size=input_size, **self.configs.model_conf)
+        elif self.configs.use_model == 'BaseModel':
+            self.model = BaseModel(input_size=input_size, **self.configs.model_conf)
         else:
             raise Exception(f'{self.configs.use_model} 模型不存在！')
         self.model.to(self.device)
         summary(self.model, input_size=(1, self.test_dataset.audio_featurizer.feature_dim))
         # 使用Pytorch2.0的编译器
         if self.configs.train_conf.use_compile and torch.__version__ >= "2" and platform.system().lower() == 'windows':
             self.model = torch.compile(self.model, mode="reduce-overhead")
         # print(self.model)
         # 获取损失函数
-        self.loss = torch.nn.CrossEntropyLoss()
+        weight = torch.tensor(self.configs.train_conf.loss_weight, dtype=torch.float, device=self.device) \
+            if self.configs.train_conf.loss_weight is not None else None
+        self.loss = torch.nn.CrossEntropyLoss(weight=weight)
         if is_train:
             if self.configs.train_conf.enable_amp:
                 self.amp_scaler = torch.cuda.amp.GradScaler(init_scale=1024)
             # 获取优化方法
             optimizer = self.configs.optimizer_conf.optimizer
             if optimizer == 'Adam':
                 self.optimizer = torch.optim.Adam(params=self.model.parameters(),
-                                                  lr=float(self.configs.optimizer_conf.learning_rate),
-                                                  weight_decay=float(self.configs.optimizer_conf.weight_decay))
+                                                  lr=self.configs.optimizer_conf.learning_rate,
+                                                  weight_decay=self.configs.optimizer_conf.weight_decay)
             elif optimizer == 'AdamW':
                 self.optimizer = torch.optim.AdamW(params=self.model.parameters(),
-                                                   lr=float(self.configs.optimizer_conf.learning_rate),
-                                                   weight_decay=float(self.configs.optimizer_conf.weight_decay))
+                                                   lr=self.configs.optimizer_conf.learning_rate,
+                                                   weight_decay=self.configs.optimizer_conf.weight_decay)
             elif optimizer == 'SGD':
                 self.optimizer = torch.optim.SGD(params=self.model.parameters(),
-                                                 momentum=self.configs.optimizer_conf.momentum,
-                                                 lr=float(self.configs.optimizer_conf.learning_rate),
-                                                 weight_decay=float(self.configs.optimizer_conf.weight_decay))
+                                                 momentum=self.configs.optimizer_conf.get('momentum', 0.9),
+                                                 lr=self.configs.optimizer_conf.learning_rate,
+                                                 weight_decay=self.configs.optimizer_conf.weight_decay)
             else:
                 raise Exception(f'不支持优化方法：{optimizer}')
             # 学习率衰减函数
             scheduler_args = self.configs.optimizer_conf.get('scheduler_args', {}) \
                 if self.configs.optimizer_conf.get('scheduler_args', {}) is not None else {}
             if self.configs.optimizer_conf.scheduler == 'CosineAnnealingLR':
                 max_step = int(self.configs.train_conf.max_epoch * 1.2) * len(self.train_loader)
@@ -238,14 +269,16 @@
             # 自动混合精度参数
             if self.amp_scaler is not None and os.path.exists(os.path.join(resume_model, 'scaler.pth')):
                 self.amp_scaler.load_state_dict(torch.load(os.path.join(resume_model, 'scaler.pth')))
             with open(os.path.join(resume_model, 'model.state'), 'r', encoding='utf-8') as f:
                 json_data = json.load(f)
                 last_epoch = json_data['last_epoch'] - 1
                 best_acc = json_data['accuracy']
+            self.optimizer.step()
+            [self.scheduler.step() for _ in range(last_epoch * len(self.train_loader))]
             logger.info('成功恢复模型参数和优化方法参数：{}'.format(resume_model))
         return last_epoch, best_acc
 
     # 保存模型
     def __save_checkpoint(self, save_model_path, epoch_id, best_acc=0., best_model=False):
         if isinstance(self.model, torch.nn.parallel.DistributedDataParallel):
             state_dict = self.model.module.state_dict()
@@ -281,16 +314,16 @@
             if os.path.exists(old_model_path):
                 shutil.rmtree(old_model_path)
         logger.info('已保存模型：{}'.format(model_path))
 
     def __train_epoch(self, epoch_id, local_rank, writer, nranks=0):
         train_times, accuracies, loss_sum = [], [], []
         start = time.time()
-        sum_batch = len(self.train_loader) * self.configs.train_conf.max_epoch
         for batch_id, (features, label, input_lens_ratio) in enumerate(self.train_loader):
+            if self.stop_train: break
             if nranks > 1:
                 features = features.to(local_rank)
                 label = label.to(local_rank).long()
             else:
                 features = features.to(self.device)
                 label = label.to(self.device).long()
             # 执行模型计算，是否开启自动混合精度
@@ -313,38 +346,39 @@
             else:
                 self.optimizer.step()
             self.optimizer.zero_grad()
 
             # 计算准确率
             acc = accuracy(output, label)
             accuracies.append(acc)
-            loss_sum.append(los)
+            loss_sum.append(los.data.cpu().numpy())
             train_times.append((time.time() - start) * 1000)
+            self.train_step += 1
 
             # 多卡训练只使用一个进程打印
             if batch_id % self.configs.train_conf.log_interval == 0 and local_rank == 0:
                 # 计算每秒训练数据量
                 train_speed = self.configs.dataset_conf.dataLoader.batch_size / (
                         sum(train_times) / len(train_times) / 1000)
                 # 计算剩余时间
-                eta_sec = (sum(train_times) / len(train_times)) * (
-                        sum_batch - (epoch_id - 1) * len(self.train_loader) - batch_id)
-                eta_str = str(timedelta(seconds=int(eta_sec / 1000)))
+                self.train_eta_sec = (sum(train_times) / len(train_times)) * (self.max_step - self.train_step) / 1000
+                eta_str = str(timedelta(seconds=int(self.train_eta_sec)))
+                self.train_loss = sum(loss_sum) / len(loss_sum)
+                self.train_acc = sum(accuracies) / len(accuracies)
                 logger.info(f'Train epoch: [{epoch_id}/{self.configs.train_conf.max_epoch}], '
                             f'batch: [{batch_id}/{len(self.train_loader)}], '
-                            f'loss: {sum(loss_sum) / len(loss_sum):.5f}, '
-                            f'accuracy: {sum(accuracies) / len(accuracies):.5f}, '
+                            f'loss: {self.train_loss:.5f}, accuracy: {self.train_acc:.5f}, '
                             f'learning rate: {self.scheduler.get_last_lr()[0]:>.8f}, '
                             f'speed: {train_speed:.2f} data/sec, eta: {eta_str}')
-                writer.add_scalar('Train/Loss', sum(loss_sum) / len(loss_sum), self.train_step)
-                writer.add_scalar('Train/Accuracy', (sum(accuracies) / len(accuracies)), self.train_step)
+                writer.add_scalar('Train/Loss', self.train_loss, self.train_log_step)
+                writer.add_scalar('Train/Accuracy', self.train_acc, self.train_log_step)
                 # 记录学习率
-                writer.add_scalar('Train/lr', self.scheduler.get_last_lr()[0], self.train_step)
-                train_times = []
-                self.train_step += 1
+                writer.add_scalar('Train/lr', self.scheduler.get_last_lr()[0], self.train_log_step)
+                train_times, accuracies, loss_sum = [], [], []
+                self.train_log_step += 1
             start = time.time()
             self.scheduler.step()
 
     def train(self,
               save_model_path='models/',
               resume_model=None,
               pretrained_model=None):
@@ -366,54 +400,61 @@
             # 初始化NCCL环境
             dist.init_process_group(backend='nccl')
             local_rank = int(os.environ["LOCAL_RANK"])
 
         # 获取数据
         self.__setup_dataloader(is_train=True)
         # 获取模型
-        self.__setup_model(input_size=self.train_dataset.audio_featurizer.feature_dim, is_train=True)
+        self.__setup_model(input_size=self.test_dataset.audio_featurizer.feature_dim, is_train=True)
 
         # 支持多卡训练
         if nranks > 1 and self.use_gpu:
             self.model.to(local_rank)
             self.model = torch.nn.parallel.DistributedDataParallel(self.model, device_ids=[local_rank])
         logger.info('训练数据：{}'.format(len(self.train_dataset)))
 
         self.__load_pretrained(pretrained_model=pretrained_model)
         # 加载恢复模型
         last_epoch, best_acc = self.__load_checkpoint(save_model_path=save_model_path, resume_model=resume_model)
 
-        test_step, self.train_step = 0, 0
+        self.train_loss, self.train_acc = None, None
+        self.eval_loss, self.eval_acc = None, None
+        self.test_log_step, self.train_log_step = 0, 0
         last_epoch += 1
         if local_rank == 0:
             writer.add_scalar('Train/lr', self.scheduler.get_last_lr()[0], last_epoch)
+        # 最大步数
+        self.max_step = len(self.train_loader) * self.configs.train_conf.max_epoch
+        self.train_step = max(last_epoch, 0) * len(self.train_loader)
         # 开始训练
         for epoch_id in range(last_epoch, self.configs.train_conf.max_epoch):
+            if self.stop_train: break
             epoch_id += 1
             start_epoch = time.time()
             # 训练一个epoch
             self.__train_epoch(epoch_id=epoch_id, local_rank=local_rank, writer=writer, nranks=nranks)
             # 多卡训练只使用一个进程执行评估和保存模型
             if local_rank == 0:
+                if self.stop_eval: continue
                 logger.info('=' * 70)
-                loss, acc = self.evaluate()
+                self.eval_loss, self.eval_acc = self.evaluate()
                 logger.info('Test epoch: {}, time/epoch: {}, loss: {:.5f}, accuracy: {:.5f}'.format(
-                    epoch_id, str(timedelta(seconds=(time.time() - start_epoch))), loss, acc))
+                    epoch_id, str(timedelta(seconds=(time.time() - start_epoch))), self.eval_loss, self.eval_acc))
                 logger.info('=' * 70)
-                writer.add_scalar('Test/Accuracy', acc, test_step)
-                writer.add_scalar('Test/Loss', loss, test_step)
-                test_step += 1
+                writer.add_scalar('Test/Accuracy', self.eval_acc, self.test_log_step)
+                writer.add_scalar('Test/Loss', self.eval_loss, self.test_log_step)
+                self.test_log_step += 1
                 self.model.train()
-                # # 保存最优模型
-                if acc >= best_acc:
-                    best_acc = acc
-                    self.__save_checkpoint(save_model_path=save_model_path, epoch_id=epoch_id, best_acc=acc,
+                # 保存最优模型
+                if self.eval_acc >= best_acc:
+                    best_acc = self.eval_acc
+                    self.__save_checkpoint(save_model_path=save_model_path, epoch_id=epoch_id, best_acc=self.eval_acc,
                                            best_model=True)
                 # 保存模型
-                self.__save_checkpoint(save_model_path=save_model_path, epoch_id=epoch_id, best_acc=acc)
+                self.__save_checkpoint(save_model_path=save_model_path, epoch_id=epoch_id, best_acc=self.eval_acc)
 
     def evaluate(self, resume_model=None, save_matrix_path=None):
         """
         评估模型
         :param resume_model: 所使用的模型
         :param save_matrix_path: 保存混合矩阵的路径
         :return: 评估结果
@@ -434,14 +475,15 @@
             eval_model = self.model.module
         else:
             eval_model = self.model
 
         accuracies, losses, preds, labels = [], [], [], []
         with torch.no_grad():
             for batch_id, (features, label, input_lens_ratio) in enumerate(tqdm(self.test_loader)):
+                if self.stop_eval: break
                 features = features.to(self.device)
                 label = label.to(self.device).long()
                 output = eval_model(features)
                 los = self.loss(output, label)
                 # 计算准确率
                 acc = accuracy(output, label)
                 accuracies.append(acc)
@@ -449,26 +491,28 @@
                 label = label.data.cpu().numpy()
                 output = output.data.cpu().numpy()
                 pred = np.argmax(output, axis=1)
                 preds.extend(pred.tolist())
                 # 真实标签
                 labels.extend(label.tolist())
                 losses.append(los.data.cpu().numpy())
-        loss = float(sum(losses) / len(losses))
-        acc = float(sum(accuracies) / len(accuracies))
+        loss = float(sum(losses) / len(losses)) if len(losses) > 0 else -1
+        acc = float(sum(accuracies) / len(accuracies)) if len(accuracies) > 0 else -1
         # 保存混合矩阵
         if save_matrix_path is not None:
-            cm = confusion_matrix(labels, preds)
-            plot_confusion_matrix(cm=cm, save_path=os.path.join(save_matrix_path, f'{int(time.time())}.png'),
-                                  class_labels=self.class_labels)
-
+            try:
+                cm = confusion_matrix(labels, preds)
+                plot_confusion_matrix(cm=cm, save_path=os.path.join(save_matrix_path, f'{int(time.time())}.png'),
+                                      class_labels=self.class_labels)
+            except Exception as e:
+                logger.error(f'保存混淆矩阵失败：{e}')
         self.model.train()
         return loss, acc
 
-    def export(self, save_model_path='models/', resume_model='models/EcapaTdnn_Fbank/best_model/'):
+    def export(self, save_model_path='models/', resume_model='models/BiLSTM_Emotion2Vec/best_model/'):
         """
         导出预测模型
         :param save_model_path: 模型保存的路径
         :param resume_model: 准备转换的模型路径
         :return:
         """
         self.__setup_model(input_size=self.test_dataset.audio_featurizer.feature_dim)
```

## mser/data_utils/audio.py

```diff
@@ -44,21 +44,21 @@
 
     def __ne__(self, other):
         """返回两个对象是否不相等"""
         return not self.__eq__(other)
 
     def __str__(self):
         """返回该音频的信息"""
-        return ("%s: num_samples=%d, sample_rate=%d, duration=%.2fsec, "
-                "rms=%.2fdB" % (type(self), self.num_samples, self.sample_rate, self.duration, self.rms_db))
+        return (f"{type(self)}: num_samples={self.num_samples}, sample_rate={self.sample_rate}, "
+                f"duration={self.duration:.2f}sec, rms={self.rms_db:.2f}dB")
 
     @classmethod
     def from_file(cls, file):
         """从音频文件创建音频段
-        
+
         :param file: 文件路径，或者文件对象
         :type file: str, BufferedReader
         :return: 音频片段实例
         :rtype: AudioSegment
         """
         assert os.path.exists(file), f'文件不存在，请检查路径：{file}'
         try:
@@ -91,17 +91,17 @@
         # 从末尾开始计
         if start < 0.0: start += duration
         if end < 0.0: end += duration
         # 保证数据不越界
         if start < 0.0: start = 0.0
         if end > duration: end = duration
         if end < 0.0:
-            raise ValueError("切片结束位置(%f s)越界" % end)
+            raise ValueError(f"切片结束位置({end} s)越界")
         if start > end:
-            raise ValueError("切片开始位置(%f s)晚于切片结束位置(%f s)" % (start, end))
+            raise ValueError(f"切片开始位置({start} s)晚于切片结束位置({end} s)")
         start_frame = int(start * sample_rate)
         end_frame = int(end * sample_rate)
         sndfile.seek(start_frame)
         data = sndfile.read(frames=end_frame - start_frame, dtype='float32')
         return cls(data, sample_rate)
 
     @classmethod
@@ -153,15 +153,15 @@
     def concatenate(cls, *segments):
         """将任意数量的音频片段连接在一起
 
         :param *segments: 输入音频片段被连接
         :type *segments: tuple of AudioSegment
         :return: Audio segment instance as concatenating results.
         :rtype: AudioSegment
-        :raises ValueError: If the number of segments is zero, or if the 
+        :raises ValueError: If the number of segments is zero, or if the
                             sample_rate of any segments does not match.
         :raises TypeError: If any segment is not AudioSegment instance.
         """
         # Perform basic sanity-checks.
         if len(segments) == 0:
             raise ValueError("没有音频片段被给予连接")
         sample_rate = segments[0]._sample_rate
@@ -185,15 +185,15 @@
         :rtype: AudioSegment
         """
         samples = np.zeros(int(duration * sample_rate))
         return cls(samples, sample_rate)
 
     def to_wav_file(self, filepath, dtype='float32'):
         """保存音频段到磁盘为wav文件
-        
+
         :param filepath: WAV文件路径或文件对象，以保存音频段
         :type filepath: str|file
         :param dtype: Subtype for audio file. Options: 'int16', 'int32',
                       'float32', 'float64'. Default is 'float32'.
         :type dtype: str
         :raises TypeError: If dtype is not supported.
         """
@@ -216,24 +216,24 @@
 
         :param other: 包含样品的片段被添加进去
         :type other: AudioSegments
         :raise TypeError: 如果两个片段的类型不匹配
         :raise ValueError: 不能添加不同类型的段
         """
         if not isinstance(other, type(self)):
-            raise TypeError("不能添加不同类型的段: %s 和 %s" % (type(self), type(other)))
+            raise TypeError(f"不能添加不同类型的段: {type(self)} 和 {type(other)}")
         if self._sample_rate != other._sample_rate:
             raise ValueError("采样率必须匹配才能添加片段")
         if len(self._samples) != len(other._samples):
             raise ValueError("段长度必须匹配才能添加段")
         self._samples += other._samples
 
     def to_bytes(self, dtype='float32'):
         """创建包含音频内容的字节字符串
-        
+
         :param dtype: Data type for export samples. Options: 'int16', 'int32',
                       'float32', 'float64'. Default is 'float32'.
         :type dtype: str
         :return: Byte string containing audio content.
         :rtype: str
         """
         samples = self._convert_samples_from_float32(self._samples, dtype)
@@ -251,19 +251,19 @@
         samples = self._convert_samples_from_float32(self._samples, dtype)
         return samples
 
     def gain_db(self, gain):
         """对音频施加分贝增益。
 
         Note that this is an in-place transformation.
-        
-        :param gain: Gain in decibels to apply to samples. 
+
+        :param gain: Gain in decibels to apply to samples.
         :type gain: float|1darray
         """
-        self._samples *= 10.**(gain / 20.)
+        self._samples *= 10. ** (gain / 20.)
 
     def change_speed(self, speed_rate):
         """通过线性插值改变音频速度
 
         :param speed_rate: Rate of speed change:
                            speed_rate > 1.0, speed up the audio;
                            speed_rate = 1.0, unchanged;
@@ -292,19 +292,17 @@
                             normalization. This is to prevent nans when
                             attempting to normalize a signal consisting of
                             all zeros.
         :type max_gain_db: float
         :raises ValueError: If the required gain to normalize the segment to
                             the target_db value exceeds max_gain_db.
         """
-        if -np.inf == self.rms_db: return
         gain = target_db - self.rms_db
         if gain > max_gain_db:
-            raise ValueError(
-                "无法将段规范化到 %f dB，因为可能的增益已经超过max_gain_db (%f dB)" % (target_db, max_gain_db))
+            raise ValueError(f"无法将段规范化到{target_db}dB，音频增益{gain}增益已经超过max_gain_db ({max_gain_db}dB)")
         self.gain_db(min(max_gain_db, target_db - self.rms_db))
 
     def resample(self, target_sample_rate, filter='kaiser_best'):
         """按目标采样率重新采样音频
 
         Note that this is an in-place transformation.
 
@@ -337,15 +335,15 @@
         if sides == "beginning":
             padded = cls.concatenate(silence, self)
         elif sides == "end":
             padded = cls.concatenate(self, silence)
         elif sides == "both":
             padded = cls.concatenate(silence, self, silence)
         else:
-            raise ValueError("Unknown value for the sides %s" % sides)
+            raise ValueError(f"Unknown value for the sides {sides}")
         self._samples = padded._samples
 
     def shift(self, shift_ms):
         """音频偏移。如果shift_ms为正，则随时间提前移位;如果为负，则随时间延迟移位。填补静音以保持持续时间不变。
 
         Note that this is an in-place transformation.
 
@@ -381,21 +379,21 @@
         start_sec = 0.0 if start_sec is None else start_sec
         end_sec = self.duration if end_sec is None else end_sec
         if start_sec < 0.0:
             start_sec = self.duration + start_sec
         if end_sec < 0.0:
             end_sec = self.duration + end_sec
         if start_sec < 0.0:
-            raise ValueError("切片起始位置(%f s)越界" % start_sec)
+            raise ValueError(f"切片起始位置({start_sec} s)越界")
         if end_sec < 0.0:
-            raise ValueError("切片结束位置(%f s)越界" % end_sec)
+            raise ValueError(f"切片结束位置({end_sec} s)越界")
         if start_sec > end_sec:
-            raise ValueError("切片的起始位置(%f s)晚于结束位置(%f s)" % (start_sec, end_sec))
+            raise ValueError(f"切片的起始位置({start_sec} s)晚于结束位置({end_sec} s)")
         if end_sec > self.duration:
-            raise ValueError("切片结束位置(%f s)越界(> %f s)" % (end_sec, self.duration))
+            raise ValueError(f"切片结束位置({end_sec} s)越界(> {self.duration} s)")
         start_sample = int(round(start_sec * self._sample_rate))
         end_sample = int(round(end_sec * self._sample_rate))
         self._samples = self._samples[start_sample:end_sample]
 
     def random_subsegment(self, subsegment_length):
         """随机剪切指定长度的音频片段
 
@@ -429,17 +427,17 @@
                             to apply infinite gain to a zero signal.
         :type max_gain_db: float
         :raises ValueError: If the sample rate does not match between the two
                             audio segments, or if the duration of noise segments
                             is shorter than original audio segments.
         """
         if noise.sample_rate != self.sample_rate:
-            raise ValueError("噪声采样率(%d Hz)不等于基信号采样率(%d Hz)" % (noise.sample_rate, self.sample_rate))
+            raise ValueError(f"噪声采样率({noise.sample_rate} Hz)不等于基信号采样率({self.sample_rate} Hz)")
         if noise.duration < self.duration:
-            raise ValueError("噪声信号(%f秒)必须至少与基信号(%f秒)一样长" % (noise.duration, self.duration))
+            raise ValueError(f"噪声信号({noise.duration}秒)必须至少与基信号({self.duration}秒)一样长")
         noise_gain_db = min(self.rms_db - noise.rms_db - snr_dB, max_gain_db)
         noise_new = copy.deepcopy(noise)
         noise_new.random_subsegment(self.duration)
         noise_new.gain_db(noise_gain_db)
         self.superimpose(noise_new)
 
     def vad(self, top_db=20, overlap=200):
@@ -494,33 +492,37 @@
         """返回以分贝为单位的音频均方根能量
 
         :return: Root mean square energy in decibels.
         :rtype: float
         """
         # square root => multiply by 10 instead of 20 for dBs
         mean_square = np.mean(self._samples ** 2)
+        if mean_square == 0:
+            mean_square = 1
         return 10 * np.log10(mean_square)
 
-    def _convert_samples_to_float32(self, samples):
+    @staticmethod
+    def _convert_samples_to_float32(samples):
         """Convert sample type to float32.
 
         Audio sample type is usually integer or float-point.
         Integers will be scaled to [-1, 1] in float32.
         """
         float32_samples = samples.astype('float32')
         if samples.dtype in np.sctypes['int']:
             bits = np.iinfo(samples.dtype).bits
             float32_samples *= (1. / 2 ** (bits - 1))
         elif samples.dtype in np.sctypes['float']:
             pass
         else:
-            raise TypeError("Unsupported sample type: %s." % samples.dtype)
+            raise TypeError(f"Unsupported sample type: {samples.dtype}.")
         return float32_samples
 
-    def _convert_samples_from_float32(self, samples, dtype):
+    @staticmethod
+    def _convert_samples_from_float32(samples, dtype):
         """Convert sample type from float32 to dtype.
 
         Audio sample type is usually integer or float-point. For integer
         type, float32 will be rescaled from [-1, 1] to the maximum range
         supported by the integer type.
 
         This is for writing a audio file.
@@ -536,9 +538,9 @@
             output_samples[output_samples < min_val] = min_val
         elif samples.dtype in np.sctypes['float']:
             min_val = np.finfo(dtype).min
             max_val = np.finfo(dtype).max
             output_samples[output_samples > max_val] = max_val
             output_samples[output_samples < min_val] = min_val
         else:
-            raise TypeError("Unsupported sample type: %s." % samples.dtype)
+            raise TypeError(f"Unsupported sample type: {samples.dtype}.")
         return output_samples.astype(dtype)
```

## mser/data_utils/featurizer.py

```diff
@@ -1,31 +1,56 @@
 import librosa
 import numpy as np
 
+from mser.utils.logger import setup_logger
+
+logger = setup_logger(__name__)
+
 
 class AudioFeaturizer(object):
     """音频特征器
 
     :param feature_method: 所使用的预处理方法
     :type feature_method: str
     :param method_args: 预处理方法的参数
     :type method_args: dict
     """
 
-    def __init__(self, feature_method='MelSpectrogram', method_args={}):
+    def __init__(self, feature_method='Emotion2Vec', method_args={}):
         super().__init__()
         self._method_args = method_args
         self._feature_method = feature_method
+        self._feature_model = None
+        logger.info(f'使用的特征方法为 {self._feature_method}')
 
     def __call__(self, x, sample_rate: float) -> np.ndarray:
-        if self._feature_method == 'CustomFeatures':
+        if self._feature_method == 'CustomFeature':
             return self.custom_features(x, sample_rate)
+        elif self._feature_method == 'Emotion2Vec':
+            return self.emotion2vec_features(x)
         else:
             raise Exception(f'预处理方法 {self._feature_method} 不存在!')
 
+    def emotion2vec_features(self, x) -> np.ndarray:
+        try:
+            from funasr import AutoModel
+        except ImportError:
+            logger.error('请先安装 funasr 库!')
+            raise ImportError('请先安装 funasr 库!')
+        if self._feature_model is None:
+            if 'granularity' not in self._method_args.keys():
+                self._method_args['granularity'] = 'utterance'
+            self._feature_model = AutoModel(model="iic/emotion2vec_base", model_revision="v2.0.4",
+                                            device='cuda',
+                                            disable_pbar=True,
+                                            disable_log=False)
+        res = self._feature_model.generate(input=[x], **self._method_args)
+        feats = res[0]["feats"]
+        return feats
+
     @staticmethod
     def custom_features(x, sample_rate: float) -> np.ndarray:
         stft = np.abs(librosa.stft(x))
 
         # fmin 和 fmax 对应于人类语音的最小最大基本频率
         pitches, magnitudes = librosa.piptrack(y=x, sr=sample_rate, S=stft, fmin=70, fmax=400)
         pitch = []
@@ -89,8 +114,13 @@
     @property
     def feature_dim(self):
         """返回特征大小
 
         :return: 特征大小
         :rtype: int
         """
-        return 312
+        if self._feature_method == 'CustomFeature':
+            return 312
+        elif self._feature_method == 'Emotion2Vec':
+            return 768
+        else:
+            raise Exception(f'预处理方法 {self._feature_method} 不存在!')
```

## mser/data_utils/reader.py

```diff
@@ -54,44 +54,46 @@
         self.num_speakers = num_speakers
         self.noises_path = None
         # 获取数据列表
         with open(data_list_path, 'r', encoding='utf-8') as f:
             self.lines = f.readlines()
         # 获取特征器
         self.audio_featurizer = audio_featurizer
-        if scaler_path:
+        if scaler_path and self.mode != 'create_data':
             self.scaler = joblib.load(scaler_path)
 
     def __getitem__(self, idx):
-        # 分割音频路径和标签
-        audio_path, label = self.lines[idx].replace('\n', '').split('\t')
-        # 读取音频
-        audio_segment = AudioSegment.from_file(audio_path)
-        # 裁剪静音
-        if self.do_vad:
-            audio_segment.vad()
-        # 数据太短不利于训练
-        if self.mode == 'train':
-            if audio_segment.duration < self.min_duration:
-                return self.__getitem__(idx + 1 if idx < len(self.lines) - 1 else 0)
-        # 重采样
-        if audio_segment.sample_rate != self._target_sample_rate:
-            audio_segment.resample(self._target_sample_rate)
-        # 音频增强
-        if self.mode == 'train':
-            audio_segment = self.augment_audio(audio_segment, **self.aug_conf)
-        # decibel normalization
-        if self._use_dB_normalization:
-            audio_segment.normalize(target_db=self._target_dB)
-        if self.max_duration > audio_segment.duration:
-            diff_duration = (self.max_duration * audio_segment.sample_rate) - audio_segment.num_samples
-            audio_segment._samples = np.pad(audio_segment.samples, (0, diff_duration), 'wrap')
-        # 裁剪需要的数据
-        audio_segment.crop(duration=self.max_duration, mode=self.mode)
-        feature = self.audio_featurizer(audio_segment.samples, sample_rate=audio_segment.sample_rate)
+        # 分割数据文件路径和标签
+        data_path, label = self.lines[idx].replace('\n', '').split('\t')
+        # 如果后缀名为.npy的文件，那么直接读取
+        if data_path.endswith('.npy'):
+            feature = np.load(data_path)
+        else:
+            # 读取音频
+            audio_segment = AudioSegment.from_file(data_path)
+            # 裁剪静音
+            if self.do_vad:
+                audio_segment.vad()
+            # 数据太短不利于训练
+            if self.mode == 'train':
+                if audio_segment.duration < self.min_duration:
+                    return self.__getitem__(idx + 1 if idx < len(self.lines) - 1 else 0)
+            # 重采样
+            if audio_segment.sample_rate != self._target_sample_rate:
+                audio_segment.resample(self._target_sample_rate)
+            # 音频增强
+            if self.mode == 'train':
+                audio_segment = self.augment_audio(audio_segment, **self.aug_conf)
+            # decibel normalization
+            if self._use_dB_normalization:
+                audio_segment.normalize(target_db=self._target_dB)
+            # 裁剪需要的数据
+            if audio_segment.duration > self.max_duration:
+                audio_segment.crop(duration=self.max_duration, mode=self.mode)
+            feature = self.audio_featurizer(audio_segment.samples, sample_rate=audio_segment.sample_rate)
         # 归一化
         if self.mode != 'create_data':
             # feature = feature - feature.mean()
             feature = self.scaler.transform([feature])
             feature = feature.squeeze().astype(np.float32)
         return np.array(feature, dtype=np.float32), np.array(int(label), dtype=np.int64)
```

## mser/utils/utils.py

```diff
@@ -51,36 +51,52 @@
         return dict_obj
     inst = Dict()
     for k, v in dict_obj.items():
         inst[k] = dict_to_object(v)
     return inst
 
 
-def plot_confusion_matrix(cm, save_path, class_labels, title='Confusion Matrix', show=False):
+def plot_confusion_matrix(cm, save_path, class_labels, show=False):
+    """
+    绘制混淆矩阵
+    @param cm: 混淆矩阵, 一个二维数组，表示预测结果与真实结果的混淆情况。
+    @param save_path: 保存路径, 字符串，指定混淆矩阵图像的保存位置。
+    @param class_labels: 类别名称, 一个列表，包含各个类别的名称。
+    @param show: 是否显示图像, 布尔值，控制是否在绘图窗口显示混淆矩阵图像。
+    """
+    # 检测类别名称是否包含中文，是则设置相应字体
+    s = ''.join(class_labels)
+    is_ascii = all(ord(c) < 128 for c in s)
+    if not is_ascii:
+        plt.rcParams['font.sans-serif'] = ['SimHei']
+        plt.rcParams['axes.unicode_minus'] = False
+
+    # 初始化绘图参数并绘制混淆矩阵
     plt.figure(figsize=(12, 8), dpi=100)
     np.set_printoptions(precision=2)
-    # 在混淆矩阵中每格的概率值
+    # 在混淆矩阵中绘制每个格子的概率值
     ind_array = np.arange(len(class_labels))
     x, y = np.meshgrid(ind_array, ind_array)
     for x_val, y_val in zip(x.flatten(), y.flatten()):
         c = cm[y_val][x_val] / (np.sum(cm[:, x_val]) + 1e-6)
-        # 忽略值太小的
+        # 忽略概率值太小的格子
         if c < 1e-4: continue
         plt.text(x_val, y_val, "%0.2f" % (c,), color='red', fontsize=15, va='center', ha='center')
-    m = np.max(cm)
+    m = np.sum(cm, axis=0) + 1e-6
     plt.imshow(cm / m, interpolation='nearest', cmap=plt.cm.binary)
-    plt.title(title)
+    plt.title('Confusion Matrix' if is_ascii else '混合矩阵')
     plt.colorbar()
+    # 设置类别标签
     xlocations = np.array(range(len(class_labels)))
     plt.xticks(xlocations, class_labels, rotation=90)
     plt.yticks(xlocations, class_labels)
-    plt.ylabel('Actual label')
-    plt.xlabel('Predict label')
+    plt.ylabel('Actual label' if is_ascii else '实际标签')
+    plt.xlabel('Predict label' if is_ascii else '预测标签')
 
-    # offset the tick
+    # 调整刻度标记位置，提高可视化效果
     tick_marks = np.array(range(len(class_labels))) + 0.5
     plt.gca().set_xticks(tick_marks, minor=True)
     plt.gca().set_yticks(tick_marks, minor=True)
     plt.gca().xaxis.set_ticks_position('none')
     plt.gca().yaxis.set_ticks_position('none')
     plt.grid(True, which='minor', linestyle='-')
     plt.gcf().subplots_adjust(bottom=0.15)
```

## Comparing `mser/models/bidirectional_lstm.py` & `mser/models/bi_lstm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch.nn as nn
 
 
-class BidirectionalLSTM(nn.Module):
+class BiLSTM(nn.Module):
     def __init__(self, input_size, num_class):
         super().__init__()
         self.fc0 = nn.Linear(in_features=input_size, out_features=512)
         self.lstm = nn.LSTM(input_size=512, hidden_size=256, bidirectional=True)
         self.tanh = nn.Tanh()
         self.dropout = nn.Dropout(p=0.5)
         self.fc1 = nn.Linear(in_features=512, out_features=256)
@@ -18,8 +18,8 @@
         y, (h, c) = self.lstm(x)
         x = y.squeeze(axis=1)
         x = self.tanh(x)
         x = self.dropout(x)
         x = self.fc1(x)
         x = self.relu1(x)
         x = self.fc2(x)
-        return x
+        return x
```

## Comparing `mser-0.0.1.dist-info/LICENSE` & `mser-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mser-0.0.1.dist-info/RECORD` & `mser-0.0.3.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-mser/__init__.py,sha256=5eB7WyFeLnIGNUDK37XonWOZZToUliGZWMZcMpjL7Og,87
-mser/predict.py,sha256=f8GkLfpTOxUN27U60Vr4T7Ur7TGUafNl7mIFhnTCmVo,7834
-mser/trainer.py,sha256=0BYU0ixnZ1HTXcH--XZ36_qjARAsb80EX0rwhCaadcw,27201
+mser/__init__.py,sha256=zkav-jYCb8ex0HaXiFdoWo9cm78reB-L2t7SnrHSGjQ,89
+mser/predict.py,sha256=_qOLEkhTQo-LHe4d4mxJ3nd8Vxo_uIcC8mc6n-8Ji7s,8006
+mser/trainer.py,sha256=559wD-46nWJ7fsYAyUIpk1CZGxyRwG-7UHGa3kWV8OA,30475
 mser/data_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mser/data_utils/audio.py,sha256=5045GFOnk3e17BLVA-UNNZE6fd4ve1hcjMNu64TzGGo,22286
+mser/data_utils/audio.py,sha256=RokQWtzrGRhdEbpl-F_t3y9FmojIXaQiOUFhYGeYgaI,22217
 mser/data_utils/collate_fn.py,sha256=GxqMcZ5Q2ScQxj6crIUWeVygzWxIk9KAbC6GWW6awrQ,965
-mser/data_utils/featurizer.py,sha256=p-kXAc9z3RE4-vMMQXv8QHVk5nBeNmp3mL1ywBIiV6I,3335
-mser/data_utils/reader.py,sha256=Y2x8m3fQ_KRpvJO3vF9wn1GReuIoi7VPOu_WF3vkMTg,6625
-mser/data_utils/spec_aug.py,sha256=Sr9-Ss6I7LA3TGMqzML_X-nb_nnMfUxt5KbsA6HJpzM,1572
+mser/data_utils/featurizer.py,sha256=ldWiJh3DT08ynFIXQ1VJyGJ_jXo3rm_xvnb-uDsjR3Q,4696
+mser/data_utils/reader.py,sha256=PV9ssBz879kCCPZ_lMxCztdF4jPobofEBDdio2nyFvc,6712
 mser/data_utils/utils.py,sha256=mNpCY4PcaeKCSjEB6gQWsiyUBRNDvwrY9YizFTRuaww,5652
 mser/metric/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mser/metric/metrics.py,sha256=Asj6VaDQXxmcB_HRIJt7v4zdRBgLTyn3Q2mDTFPcgEM,329
 mser/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mser/models/bidirectional_lstm.py,sha256=EciYVB9I49-olVx04wjGt6_TPmqgabdNxfYTBEuLHGg,854
+mser/models/base_model.py,sha256=KqLkZdovsSHGtVih5i8MafaSE6xsfbb00y93POb8v5s,420
+mser/models/bi_lstm.py,sha256=OSAivQBsU3djN93k-WOBnjLZV_CzBAuDJBFp0R1tROY,845
 mser/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mser/utils/logger.py,sha256=-ssorx8FlHA_wrd2Eq6f4HkOqaOG2YseBGvYAo8NXN8,2839
 mser/utils/record.py,sha256=2i4kz5kPDa9KkbAK_Q34sVIXOkD9TroPROIe5QdzqWg,1067
 mser/utils/scheduler.py,sha256=RXgRf_sntkOjruj30pp6uPE7dqFR06jDa4tRogpl5Us,1496
-mser/utils/utils.py,sha256=15e0VJw48zoZpNpLhxaoo7iv-BBkWXERknbDIodJX18,3363
-mser-0.0.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-mser-0.0.1.dist-info/METADATA,sha256=iVqx2vSIMNgxG_ALNJlP23hB8K_EjeXnytszzfq6OGo,11302
-mser-0.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mser-0.0.1.dist-info/top_level.txt,sha256=rK-UG_nYhj24zLM6SutX-lIidggJ9s-P3xZ6UqKEyl0,5
-mser-0.0.1.dist-info/RECORD,,
+mser/utils/utils.py,sha256=zf45Ooet18OJi-9TmaK_PI4mo-gccJL0CmLXKXXg_LM,4299
+mser-0.0.3.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+mser-0.0.3.dist-info/METADATA,sha256=16WqIsvz4_U9d7SiCcTZ7Iev4tkP-I8U3mzXOpPPkvc,18150
+mser-0.0.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+mser-0.0.3.dist-info/top_level.txt,sha256=rK-UG_nYhj24zLM6SutX-lIidggJ9s-P3xZ6UqKEyl0,5
+mser-0.0.3.dist-info/RECORD,,
```

