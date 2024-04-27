# Comparing `tmp/mvector-1.0.1-py3-none-any.whl.zip` & `tmp/mvector-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 61442 bytes, number of entries: 32
--rw-rw-rw-  2.0 fat      134 b- defN 24-Jan-10 12:54 mvector/__init__.py
+Zip file size: 60157 bytes, number of entries: 32
+-rw-rw-rw-  2.0 fat      134 b- defN 24-Apr-27 06:43 mvector/__init__.py
 -rw-rw-rw-  2.0 fat    17707 b- defN 24-Jan-10 12:54 mvector/predict.py
--rw-rw-rw-  2.0 fat    38682 b- defN 24-Jan-10 12:54 mvector/trainer.py
+-rw-rw-rw-  2.0 fat    35940 b- defN 24-Apr-27 06:40 mvector/trainer.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Jan-06 05:59 mvector/data_utils/__init__.py
--rw-rw-rw-  2.0 fat    22281 b- defN 24-Jan-06 05:59 mvector/data_utils/audio.py
+-rw-rw-rw-  2.0 fat    22220 b- defN 24-Apr-27 05:32 mvector/data_utils/audio.py
 -rw-rw-rw-  2.0 fat      965 b- defN 24-Jan-06 05:59 mvector/data_utils/collate_fn.py
 -rw-rw-rw-  2.0 fat     3587 b- defN 24-Jan-06 05:59 mvector/data_utils/featurizer.py
 -rw-rw-rw-  2.0 fat     5885 b- defN 24-Jan-06 05:59 mvector/data_utils/reader.py
 -rw-rw-rw-  2.0 fat     1572 b- defN 24-Jan-06 05:59 mvector/data_utils/spec_aug.py
 -rw-rw-rw-  2.0 fat     4712 b- defN 24-Jan-06 05:59 mvector/data_utils/utils.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Jan-06 05:59 mvector/metric/__init__.py
 -rw-rw-rw-  2.0 fat     1517 b- defN 24-Jan-06 05:59 mvector/metric/metrics.py
@@ -19,16 +19,16 @@
 -rw-rw-rw-  2.0 fat     9448 b- defN 24-Jan-10 12:54 mvector/models/loss.py
 -rw-rw-rw-  2.0 fat     3795 b- defN 24-Jan-06 05:59 mvector/models/pooling.py
 -rw-rw-rw-  2.0 fat     6687 b- defN 24-Jan-06 05:59 mvector/models/res2net.py
 -rw-rw-rw-  2.0 fat     5522 b- defN 24-Jan-06 05:59 mvector/models/resnet_se.py
 -rw-rw-rw-  2.0 fat     2963 b- defN 24-Jan-06 05:59 mvector/models/tdnn.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Jan-06 05:59 mvector/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2839 b- defN 24-Jan-06 05:59 mvector/utils/logger.py
--rw-rw-rw-  2.0 fat     1067 b- defN 24-Jan-06 05:59 mvector/utils/record.py
+-rw-rw-rw-  2.0 fat     1385 b- defN 24-Jan-15 12:44 mvector/utils/record.py
 -rw-rw-rw-  2.0 fat     3538 b- defN 24-Jan-06 05:59 mvector/utils/scheduler.py
 -rw-rw-rw-  2.0 fat     2789 b- defN 24-Jan-06 05:59 mvector/utils/utils.py
--rw-rw-rw-  2.0 fat    11558 b- defN 24-Jan-14 08:09 mvector-1.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    34567 b- defN 24-Jan-14 08:09 mvector-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Jan-14 08:09 mvector-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Jan-14 08:09 mvector-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2595 b- defN 24-Jan-14 08:09 mvector-1.0.1.dist-info/RECORD
-32 files, 217295 bytes uncompressed, 57314 bytes compressed:  73.6%
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-27 06:43 mvector-1.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    32558 b- defN 24-Apr-27 06:43 mvector-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-27 06:43 mvector-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-27 06:43 mvector-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2595 b- defN 24-Apr-27 06:43 mvector-1.0.2.dist-info/RECORD
+32 files, 212801 bytes uncompressed, 56029 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -75,23 +75,23 @@
 
 Filename: mvector/utils/scheduler.py
 Comment: 
 
 Filename: mvector/utils/utils.py
 Comment: 
 
-Filename: mvector-1.0.1.dist-info/LICENSE
+Filename: mvector-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: mvector-1.0.1.dist-info/METADATA
+Filename: mvector-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: mvector-1.0.1.dist-info/WHEEL
+Filename: mvector-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: mvector-1.0.1.dist-info/top_level.txt
+Filename: mvector-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mvector-1.0.1.dist-info/RECORD
+Filename: mvector-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mvector/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 # 项目支持的模型
 SUPPORT_MODEL = ['ERes2Net', 'CAMPPlus', 'EcapaTdnn', 'Res2Net', 'ResNetSE', 'TDNN']
```

## mvector/trainer.py

```diff
@@ -59,32 +59,34 @@
                 configs = yaml.load(f.read(), Loader=yaml.FullLoader)
             print_arguments(configs=configs)
         self.configs = dict_to_object(configs)
         assert self.configs.use_model in SUPPORT_MODEL, f'没有该模型：{self.configs.use_model}'
         self.model = None
         self.backbone = None
         self.model_output_name = '1.weight'
-        self.train_method = None
-        self.original_weight = {}
-        self.old_num_class = None
         self.enroll_loader = None
         self.trials_loader = None
         self.margin_scheduler = None
         self.amp_scaler = None
         # 获取特征器
         self.audio_featurizer = AudioFeaturizer(feature_method=self.configs.preprocess_conf.feature_method,
                                                 method_args=self.configs.preprocess_conf.get('method_args', {}))
         self.audio_featurizer.to(self.device)
         # 特征增强
         self.spec_aug = SpecAug(**self.configs.dataset_conf.get('spec_aug_args', {}))
         self.spec_aug.to(self.device)
-
         if platform.system().lower() == 'windows':
             self.configs.dataset_conf.dataLoader.num_workers = 0
             logger.warning('Windows系统不支持多线程读取数据，已自动关闭！')
+        self.max_step, self.train_step = None, None
+        self.train_loss, self.train_acc = None, None
+        self.train_eta_sec = None
+        self.eval_eer, self.eval_min_dcf, self.eval_threshold = None, None, None
+        self.test_log_step, self.train_log_step = 0, 0
+        self.stop_train, self.stop_eval = False, False
 
     def __setup_dataloader(self, is_train=False):
         if is_train:
             self.train_dataset = CustomDataset(data_list_path=self.configs.dataset_conf.train_list,
                                                do_vad=self.configs.dataset_conf.do_vad,
                                                max_duration=self.configs.dataset_conf.max_duration,
                                                min_duration=self.configs.dataset_conf.min_duration,
@@ -150,20 +152,16 @@
         if is_train:
             if self.configs.train_conf.enable_amp:
                 self.amp_scaler = torch.cuda.amp.GradScaler(init_scale=1024)
             use_loss = self.configs.loss_conf.get('use_loss', 'AAMLoss')
             # 获取分类器
             num_class = self.configs.model_conf.classifier.num_speakers
             # 语速扰动要增加分类数量
-            if self.configs.dataset_conf.aug_conf.speed_perturb:
-                if self.train_method is not None:
-                    assert not self.configs.dataset_conf.aug_conf.speed_perturb_3_class, \
-                        '增量学习不能使用语速扰动增加分类数量'
-                if self.configs.dataset_conf.aug_conf.speed_perturb_3_class:
-                    self.configs.model_conf.classifier.num_speakers = num_class * 3
+            self.configs.model_conf.classifier.num_speakers = num_class * 3 \
+                if self.configs.dataset_conf.aug_conf.speed_perturb else num_class
             # 分类器
             classifier = SpeakerIdentification(input_dim=self.backbone.embd_dim,
                                                loss_type=use_loss,
                                                **self.configs.model_conf.classifier)
             # 合并模型
             self.model = nn.Sequential(self.backbone, classifier)
             # print(self.model)
@@ -234,65 +232,33 @@
             self.model.to(self.device)
         self.model.to(self.device)
         summary(self.model, (1, 98, self.audio_featurizer.feature_dim))
         # 使用Pytorch2.0的编译器
         if self.configs.train_conf.use_compile and torch.__version__ >= "2" and platform.system().lower() != 'windows':
             self.model = torch.compile(self.model, mode="reduce-overhead")
 
-    # 改变分类器输出权重大小
-    def __change_model_output_size(self, model_state_dict, hp_alpha=0.2):
-        if self.model_output_name not in model_state_dict.keys():
-            return model_state_dict
-        self.old_num_class = model_state_dict[self.model_output_name].size(0)
-        new_num_class = self.configs.model_conf.classifier.num_speakers
-        logger.info(f'【增量学习】改变分类器输出权重大小，原分类器输出大小：{self.old_num_class}, 新分类器输出大小：{new_num_class}')
-
-        output = model_state_dict[self.model_output_name]
-        position_ids = torch.LongTensor(list(range(new_num_class)))
-        i = position_ids // self.old_num_class
-        j = position_ids % self.old_num_class
-        base_output = (output - output[0:1] * hp_alpha) / (1 - hp_alpha)
-
-        position_output = hp_alpha * base_output[i] + (1 - hp_alpha) * base_output[j]
-        model_state_dict[self.model_output_name] = position_output
-        return model_state_dict
-
-    # 加载预训练模型
     def __load_pretrained(self, pretrained_model):
-        if self.train_method is not None:
-            assert pretrained_model is not None, '增量学习必须要设置预训练模型!'
-        if pretrained_model is not None:
-            if os.path.isdir(pretrained_model):
-                pretrained_model = os.path.join(pretrained_model, 'model.pth')
-            assert os.path.exists(pretrained_model), f"{pretrained_model} 模型不存在！"
-            model_state_dict = torch.load(pretrained_model)
-            # 增量学习改变分类器输出权重大小
-            if self.train_method is not None:
-                model_state_dict = self.__change_model_output_size(model_state_dict)
-                # 获取原始的模型参数，用于计算增量学习损失
-                for param_name, param in model_state_dict.items():
-                    self.original_weight[param_name] = param.data.clone()
-            else:
-                for param_name, param in self.model.named_parameters():
-                    if param_name in model_state_dict.keys() and model_state_dict[param_name].size() != param.size():
-                        logger.warning(f'模型参数{param_name}的大小不匹配，权重的是{model_state_dict[param_name].size()}, '
-                                       f'模型的是{param.size()}，已忽略！')
-                        del model_state_dict[param_name]
-            # 加载权重
-            if isinstance(self.model, torch.nn.parallel.DistributedDataParallel):
-                missing_keys, unexpected_keys = self.model.module.load_state_dict(model_state_dict, strict=False)
-            else:
-                missing_keys, unexpected_keys = self.model.load_state_dict(model_state_dict, strict=False)
-            if len(unexpected_keys) > 0:
-                logger.warning('Unexpected key(s) in state_dict: {}. '
-                               .format(', '.join('"{}"'.format(k) for k in unexpected_keys)))
-            if len(missing_keys) > 0:
-                logger.warning('Missing key(s) in state_dict: {}. '
-                               .format(', '.join('"{}"'.format(k) for k in missing_keys)))
-            logger.info('成功加载预训练模型：{}'.format(pretrained_model))
+        # 加载预训练模型
+        if pretrained_model is None: return
+        if os.path.isdir(pretrained_model):
+            pretrained_model = os.path.join(pretrained_model, 'model.pth')
+        assert os.path.exists(pretrained_model), f"{pretrained_model} 模型不存在！"
+        model_state_dict = torch.load(pretrained_model)
+        # 加载权重
+        if isinstance(self.model, torch.nn.parallel.DistributedDataParallel):
+            missing_keys, unexpected_keys = self.model.module.load_state_dict(model_state_dict, strict=False)
+        else:
+            missing_keys, unexpected_keys = self.model.load_state_dict(model_state_dict, strict=False)
+        if len(unexpected_keys) > 0:
+            logger.warning('Unexpected key(s) in state_dict: {}. '
+                           .format(', '.join('"{}"'.format(k) for k in unexpected_keys)))
+        if len(missing_keys) > 0:
+            logger.warning('Missing key(s) in state_dict: {}. '
+                           .format(', '.join('"{}"'.format(k) for k in missing_keys)))
+        logger.info('成功加载预训练模型：{}'.format(pretrained_model))
 
     def __load_checkpoint(self, save_model_path, resume_model):
         last_epoch = -1
         best_eer = 1
         last_model_dir = os.path.join(save_model_path,
                                       f'{self.configs.use_model}_{self.configs.preprocess_conf.feature_method}',
                                       'last_model')
@@ -314,15 +280,19 @@
             with open(os.path.join(resume_model, 'model.state'), 'r', encoding='utf-8') as f:
                 json_data = json.load(f)
                 last_epoch = json_data['last_epoch'] - 1
                 if 'eer' in json_data.keys():
                     best_eer = json_data['eer']
             logger.info('成功恢复模型参数和优化方法参数：{}'.format(resume_model))
             self.optimizer.step()
-            [self.scheduler.step() for _ in range(last_epoch * len(self.train_loader))]
+            # 恢复学习率和margin
+            if last_epoch >= 0:
+                [self.scheduler.step() for _ in range((last_epoch + 1) * len(self.train_loader))]
+                if self.margin_scheduler:
+                    self.margin_scheduler.step((last_epoch + 1) * len(self.train_loader))
         return last_epoch, best_eer
 
     # 保存模型
     def __save_checkpoint(self, save_model_path, epoch_id, eer=None, min_dcf=None, threshold=None, best_model=False):
         if isinstance(self.model, torch.nn.parallel.DistributedDataParallel):
             state_dict = self.model.module.state_dict()
         else:
@@ -343,14 +313,16 @@
             torch.save(self.amp_scaler.state_dict(), os.path.join(model_path, 'scaler.pth'))
         with open(os.path.join(model_path, 'model.state'), 'w', encoding='utf-8') as f:
             data = {"last_epoch": epoch_id, "version": __version__}
             if eer is not None:
                 data['threshold'] = threshold
                 data['eer'] = eer
                 data['min_dcf'] = min_dcf
+            if self.margin_scheduler:
+                data['margin'] = self.margin_scheduler.get_margin()
             f.write(json.dumps(data, ensure_ascii=False))
         if not best_model:
             last_model_path = os.path.join(save_model_path,
                                            f'{self.configs.use_model}_{self.configs.preprocess_conf.feature_method}',
                                            'last_model')
             shutil.rmtree(last_model_path, ignore_errors=True)
             shutil.copytree(model_path, last_model_path)
@@ -358,20 +330,20 @@
             old_model_path = os.path.join(save_model_path,
                                           f'{self.configs.use_model}_{self.configs.preprocess_conf.feature_method}',
                                           'epoch_{}'.format(epoch_id - 3))
             if os.path.exists(old_model_path):
                 shutil.rmtree(old_model_path)
         logger.info('已保存模型：{}'.format(model_path))
 
-    def __train_epoch(self, epoch_id, save_model_path, local_rank, writer, nranks=0, il_ratio=10.0):
-        train_times, accuracies, loss_sum, il_losses = [], [], [], []
+    def __train_epoch(self, epoch_id, save_model_path, local_rank, writer, nranks=0):
+        train_times, accuracies, loss_sum = [], [], []
         start = time.time()
         use_loss = self.configs.loss_conf.get('use_loss', 'AAMLoss')
-        sum_batch = len(self.train_loader) * self.configs.train_conf.max_epoch
         for batch_id, (audio, label, input_lens_ratio) in enumerate(self.train_loader):
+            if self.stop_train: break
             if nranks > 1:
                 audio = audio.to(local_rank)
                 input_lens_ratio = input_lens_ratio.to(local_rank)
                 label = label.to(local_rank).long()
             else:
                 audio = audio.to(self.device)
                 input_lens_ratio = input_lens_ratio.to(self.device)
@@ -381,28 +353,14 @@
             if self.configs.dataset_conf.use_spec_aug:
                 features = self.spec_aug(features)
             # 执行模型计算，是否开启自动混合精度
             with torch.cuda.amp.autocast(enabled=self.configs.train_conf.enable_amp):
                 output = self.model(features)
             # 计算损失值
             los = self.loss(output, label)
-            # 增量学习损失
-            if self.train_method == 'ewc':
-                losses = []
-                for n, p in self.model.named_parameters():
-                    # 每个参数都有mean和fisher
-                    mean = self.original_weight[n.replace("module.", "")]
-                    if self.model_output_name == n:
-                        pass
-                        # losses.append(((p - mean)[:self.old_num_class, :] ** 2).sum())
-                    else:
-                        losses.append(((p - mean) ** 2).sum())
-                ewc_loss = sum(losses)
-                los = los + (ewc_loss * il_ratio)
-                il_losses.append(ewc_loss * il_ratio)
             # 是否开启自动混合精度
             if self.configs.train_conf.enable_amp:
                 # loss缩放，乘以系数loss_scaling
                 scaled = self.amp_scaler.scale(los)
                 scaled.backward()
             else:
                 los.backward()
@@ -420,67 +378,59 @@
                 loss_args = self.configs.loss_conf.get('args', {})
                 cosine = torch.reshape(output, (-1, output.shape[1] // loss_args.K, loss_args.K))
                 output, _ = torch.max(cosine, 2)
             acc = accuracy(output, label)
             accuracies.append(acc)
             loss_sum.append(los.data.cpu().numpy())
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
-                il_loss_str = f'il_loss: {sum(il_losses) / len(il_losses):.5f}, ' if self.train_method is not None else ''
+                self.train_eta_sec = (sum(train_times) / len(train_times)) * (self.max_step - self.train_step) / 1000
+                eta_str = str(timedelta(seconds=int(self.train_eta_sec)))
+                self.train_loss = sum(loss_sum) / len(loss_sum)
+                self.train_acc = sum(accuracies) / len(accuracies)
                 logger.info(f'Train epoch: [{epoch_id}/{self.configs.train_conf.max_epoch}], '
                             f'batch: [{batch_id}/{len(self.train_loader)}], '
-                            f'loss: {sum(loss_sum) / len(loss_sum):.5f}, {il_loss_str}'
-                            f'accuracy: {sum(accuracies) / len(accuracies):.5f}, '
-                            f'learning rate: {self.scheduler.get_last_lr()[0]:>.8f}, '
+                            f'loss: {self.train_loss:.5f}, accuracy: {self.train_acc:.5f}, '
+                            f'learning rate: {self.scheduler.get_last_lr()[0]:.8f}, '
                             f'speed: {train_speed:.2f} data/sec, eta: {eta_str}')
-                writer.add_scalar('Train/Loss', sum(loss_sum) / len(loss_sum), self.train_step)
-                if self.train_method is not None:
-                    writer.add_scalar('Train/il_loss', sum(il_losses) / len(il_losses), self.train_step)
-                writer.add_scalar('Train/Accuracy', (sum(accuracies) / len(accuracies)), self.train_step)
+                writer.add_scalar('Train/Loss', self.train_loss, self.train_log_step)
+                writer.add_scalar('Train/Accuracy', self.train_acc, self.train_log_step)
                 # 记录学习率
-                writer.add_scalar('Train/lr', self.scheduler.get_last_lr()[0], self.train_step)
-                self.train_step += 1
+                writer.add_scalar('Train/lr', self.scheduler.get_last_lr()[0], self.train_log_step)
+                if self.margin_scheduler:
+                    writer.add_scalar('Train/margin', self.margin_scheduler.get_margin(), self.train_log_step)
+                self.train_log_step += 1
                 train_times, accuracies, loss_sum = [], [], []
             # 固定步数也要保存一次模型
             if batch_id % 10000 == 0 and batch_id != 0 and local_rank == 0:
                 self.__save_checkpoint(save_model_path=save_model_path, epoch_id=epoch_id)
             start = time.time()
             self.scheduler.step()
             if self.margin_scheduler:
                 self.margin_scheduler.step()
 
     def train(self,
               save_model_path='models/',
               resume_model=None,
               pretrained_model=None,
-              do_eval=True,
-              train_method=None,
-              il_ratio=1.0):
+              do_eval=True):
         """
         训练模型
         :param save_model_path: 模型保存的路径
         :param resume_model: 恢复训练，当为None则不使用预训练模型
         :param pretrained_model: 预训练模型的路径，当为None则不使用预训练模型
         :param do_eval: 训练时是否评估模型
-        :param train_method: 增量学习方法，为None则不使用增量学习
-        :param il_ratio: 增量学习损失的权重
         """
-        assert train_method in ['ewc', None]
-        self.train_method = train_method
-        if self.train_method is not None:
-            logger.info(f'增量学习，增量学习方法: {train_method}')
         # 获取有多少张显卡训练
         nranks = torch.cuda.device_count()
         local_rank = 0
         writer = None
         if local_rank == 0:
             # 日志记录器
             writer = LogWriter(logdir='log')
@@ -491,65 +441,67 @@
             local_rank = int(os.environ["LOCAL_RANK"])
         # 获取数据
         self.__setup_dataloader(is_train=True)
         # 获取模型
         self.__setup_model(input_size=self.audio_featurizer.feature_dim, is_train=True)
         # 加载预训练模型
         self.__load_pretrained(pretrained_model=pretrained_model)
-        # 获取原始的模型参数，用于计算增量学习损失
-        if self.train_method is not None:
-            for param_name, param in self.model.named_parameters():
-                self.original_weight[param_name] = param.data.clone()
         # 加载恢复模型
         last_epoch, best_eer = self.__load_checkpoint(save_model_path=save_model_path, resume_model=resume_model)
         if last_epoch > 0:
             self.optimizer.step()
             [self.scheduler.step() for _ in range(last_epoch)]
 
         # 支持多卡训练
         if nranks > 1 and self.use_gpu:
             self.model.to(local_rank)
             self.audio_featurizer.to(local_rank)
             self.model = torch.nn.parallel.DistributedDataParallel(self.model, device_ids=[local_rank])
         logger.info('训练数据：{}'.format(len(self.train_dataset)))
 
-        eer, min_dcf, threshold = None, None, None
-        test_step, self.train_step = 0, 0
+        self.train_loss, self.train_acc = None, None
+        self.test_log_step, self.train_log_step = 0, 0
+        self.eval_eer, self.eval_min_dcf, self.eval_threshold = None, None, None
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
             self.__train_epoch(epoch_id=epoch_id, save_model_path=save_model_path, local_rank=local_rank,
-                               writer=writer, nranks=nranks, il_ratio=il_ratio)
+                               writer=writer, nranks=nranks)
             # 多卡训练只使用一个进程执行评估和保存模型
             if local_rank == 0 and do_eval:
+                if self.stop_eval: continue
                 logger.info('=' * 70)
-                eer, min_dcf, threshold = self.evaluate()
+                self.eval_eer, self.eval_min_dcf, self.eval_threshold = self.evaluate()
                 logger.info('Test epoch: {}, time/epoch: {}, threshold: {:.2f}, EER: {:.5f}, '
                             'MinDCF: {:.5f}'.format(epoch_id, str(timedelta(
-                    seconds=(time.time() - start_epoch))), threshold, eer, min_dcf))
+                    seconds=(time.time() - start_epoch))), self.eval_threshold, self.eval_eer, self.eval_min_dcf))
                 logger.info('=' * 70)
-                writer.add_scalar('Test/threshold', threshold, test_step)
-                writer.add_scalar('Test/min_dcf', min_dcf, test_step)
-                writer.add_scalar('Test/eer', eer, test_step)
-                test_step += 1
+                writer.add_scalar('Test/threshold', self.eval_threshold, self.test_log_step)
+                writer.add_scalar('Test/min_dcf', self.eval_min_dcf, self.test_log_step)
+                writer.add_scalar('Test/eer', self.eval_eer, self.test_log_step)
+                self.test_log_step += 1
                 self.model.train()
                 # # 保存最优模型
-                if eer <= best_eer:
-                    best_eer = eer
-                    self.__save_checkpoint(save_model_path=save_model_path, epoch_id=epoch_id, eer=eer, min_dcf=min_dcf,
-                                           threshold=threshold, best_model=True)
+                if self.eval_eer <= best_eer:
+                    best_eer = self.eval_eer
+                    self.__save_checkpoint(save_model_path=save_model_path, epoch_id=epoch_id, eer=self.eval_eer,
+                                           min_dcf=self.eval_min_dcf, threshold=self.eval_threshold, best_model=True)
             if local_rank == 0:
                 # 保存模型
-                self.__save_checkpoint(save_model_path=save_model_path, epoch_id=epoch_id, eer=eer, min_dcf=min_dcf,
-                                       threshold=threshold)
+                self.__save_checkpoint(save_model_path=save_model_path, epoch_id=epoch_id, eer=self.eval_eer,
+                                       min_dcf=self.eval_min_dcf, threshold=self.eval_threshold)
 
     def evaluate(self, resume_model=None, save_image_path=None):
         """
         评估模型
         :param resume_model: 所使用的模型
         :param save_image_path: 保存图片的路径
         :return: 评估结果
@@ -576,30 +528,30 @@
             eval_model = self.model.module if len(self.model.module) == 1 else self.model.module[0]
         else:
             eval_model = self.model if len(self.model) == 1 else self.model[0]
 
         # 获取注册的声纹特征和标签
         enroll_features, enroll_labels = None, None
         with torch.no_grad():
-            for batch_id, (audio, label, input_lens_ratio) in enumerate(
-                    tqdm(self.enroll_loader, desc="注册音频声纹特征")):
+            for batch_id, (audio, label, input_lens_ratio) in enumerate(tqdm(self.enroll_loader, desc="注册音频声纹特征")):
+                if self.stop_eval: break
                 audio = audio.to(self.device)
                 input_lens_ratio = input_lens_ratio.to(self.device)
                 label = label.to(self.device).long()
                 audio_features, _ = self.audio_featurizer(audio, input_lens_ratio)
                 feature = eval_model(audio_features).data.cpu().numpy()
                 label = label.data.cpu().numpy()
                 # 存放特征
                 enroll_features = np.concatenate((enroll_features, feature)) if enroll_features is not None else feature
                 enroll_labels = np.concatenate((enroll_labels, label)) if enroll_labels is not None else label
         # 获取检验的声纹特征和标签
         trials_features, trials_labels = None, None
         with torch.no_grad():
-            for batch_id, (audio, label, input_lens_ratio) in enumerate(
-                    tqdm(self.trials_loader, desc="验证音频声纹特征")):
+            for batch_id, (audio, label, input_lens_ratio) in enumerate(tqdm(self.trials_loader, desc="验证音频声纹特征")):
+                if self.stop_eval: break
                 audio = audio.to(self.device)
                 input_lens_ratio = input_lens_ratio.to(self.device)
                 label = label.to(self.device).long()
                 audio_features, _ = self.audio_featurizer(audio, input_lens_ratio)
                 feature = eval_model(audio_features).data.cpu().numpy()
                 label = label.data.cpu().numpy()
                 # 存放特征
@@ -607,20 +559,22 @@
                 trials_labels = np.concatenate((trials_labels, label)) if trials_labels is not None else label
         self.model.train()
         enroll_labels = enroll_labels.astype(np.int32)
         trials_labels = trials_labels.astype(np.int32)
         print('开始对比音频特征...')
         all_score, all_labels = [], []
         for i in tqdm(range(len(trials_features)), desc='特征对比'):
+            if self.stop_eval: break
             trials_feature = np.expand_dims(trials_features[i], 0).repeat(len(enroll_features), axis=0)
             score = cosine_similarity(trials_feature, enroll_features).tolist()[0]
             trials_label = np.expand_dims(trials_labels[i], 0).repeat(len(enroll_features), axis=0)
             y_true = np.array(enroll_labels == trials_label).astype(np.int32).tolist()
             all_score.extend(score)
             all_labels.extend(y_true)
+        if self.stop_eval: return -1, -1, -1,
         # 计算EER
         all_score = np.array(all_score)
         all_labels = np.array(all_labels)
         fnr, fpr, thresholds = compute_fnr_fpr(all_score, all_labels)
         eer, threshold = compute_eer(fnr, fpr, all_score)
         min_dcf = compute_dcf(fnr, fpr)
```

## mvector/data_utils/audio.py

```diff
@@ -44,16 +44,16 @@
 
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
 
         :param file: 文件路径，或者文件对象
         :type file: str, BufferedReader
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

## mvector/utils/record.py

```diff
@@ -1,8 +1,9 @@
 import os
+import time
 
 import soundcard
 import soundfile
 
 
 class RecordAudio:
     def __init__(self, channels=1, sample_rate=16000):
@@ -18,14 +19,18 @@
 
         :param record_seconds: 录音时间，默认3秒
         :param save_path: 录音保存的路径，后缀名为wav
         :return: 音频的numpy数据
         """
         print("开始录音......")
         num_frames = int(record_seconds * self.sample_rate)
+        start_time = time.time()
         data = self.default_mic.record(samplerate=self.sample_rate, numframes=num_frames, channels=self.channels)
+        if int(time.time() - start_time) < record_seconds:
+            raise Exception('录音错误，请检查录音设备，或者卸载soundfile，使用命令重新安装：'
+                            'pip install git+https://github.com/bastibe/SoundCard.git')
         audio_data = data.squeeze()
         print("录音已结束!")
         if save_path is not None:
             os.makedirs(os.path.dirname(save_path), exist_ok=True)
             soundfile.write(save_path, data=data, samplerate=self.sample_rate)
         return audio_data
```

## Comparing `mvector-1.0.1.dist-info/LICENSE` & `mvector-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mvector-1.0.1.dist-info/METADATA` & `mvector-1.0.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvector
-Version: 1.0.1
+Version: 1.0.2
 Summary: Voice Print Recognition toolkit on Pytorch
 Home-page: https://github.com/yeyupiaoling/VoiceprintRecognition_Pytorch
 Download-URL: https://github.com/yeyupiaoling/VoiceprintRecognition_Pytorch.git
 Author: yeyupiaoling
 License: Apache License 2.0
 Keywords: Voice,Pytorch
 Classifier: Intended Audience :: Developers
@@ -383,14 +383,18 @@
 ······································································
 W0425 08:29:10.006249 21121 device_context.cc:447] Please NOTE: device: 0, GPU Compute Capability: 7.5, Driver API Version: 11.6, Runtime API Version: 10.2
 W0425 08:29:10.008555 21121 device_context.cc:465] device: 0, cuDNN Version: 7.6.
 成功加载模型参数和优化方法参数：models/EcapaTdnn_Fbank/best_model/model.pth
 audio/a_1.wav 和 audio/b_2.wav 不是同一个人，相似度为：-0.09565544128417969
 ```
 
+同时还提供了有GUI界面的声纹对比程序，执行`infer_contrast_gui.py`启动程序，界面如下，分别选择两个音频，点击开始判断，就可以判断它们是否是同一个人。
+
+<img src="./docs/images/contrast.jpg" alt="声纹对比界面">
+
 # 声纹识别
 
 在新闻识别里面主要使用到`register()`函数和`recognition()`函数，首先使用`register()`函数函数来注册音频到声纹库里面，也可以直接把文件添加到`audio_db`文件夹里面，使用的时候通过`recognition()`函数来发起识别，输入一条音频，就可以从声纹库里面识别到所需要的说话人。
 
 有了上面的声纹识别的函数，读者可以根据自己项目的需求完成声纹识别的方式，例如笔者下面提供的是通过录音来完成声纹识别。首先必须要加载语音库中的语音，语音库文件夹为`audio_db`，然后用户回车后录音3秒钟，然后程序会自动录音，并使用录音到的音频进行声纹识别，去匹配语音库中的语音，获取用户的信息。通过这样方式，读者也可以修改成通过服务请求的方式完成声纹识别，例如提供一个API供APP调用，用户在APP上通过声纹登录时，把录音到的语音发送到后端完成声纹识别，再把结果返回给APP，前提是用户已经使用语音注册，并成功把语音数据存放在`audio_db`文件夹中。
 ```shell
 python infer_recognition.py
@@ -420,53 +424,19 @@
 请选择功能，0为注册音频到声纹库，1为执行声纹识别：1
 按下回车键开机录音，录音3秒中：
 开始录音......
 录音已结束!
 识别说话的为：夜雨飘零，相似度为：0.920434
 ```
 
-# 增量学习 (效果不好)
-
-增量学习是为了克服在训练新数据的时候对旧数据出现灾难性遗忘，如果在声纹识别模型中只单纯微调新数据，直接修改模型的输出大小，反而会导致整个模型性能下降，甚至完全不可用。为了避免这种情况出现，本项目提供了增量学习的方法，即使在没有原数据集的情况下，也可以训练私有数据，在提高私有数据集准确率的情况下，也不会严重影响模型本身的性能。
-
-1. 首先要确保网络结构是一样的，除了最后的分类大小不一样，其他都一样。也就是说跟模型权重配套的配置文件中，模型参数只允许修改`num_speakers`参数，其他的`model_conf`参数不能修改。
-2. 增量学习中，不能使用语速增强增加说话人数量，也就是说`speed_perturb_3_class`参数必须为False。
-3. 在生成数据列表的时候，开始的标签必须是原模型的分类大小，而不是0，如果不知道原模型的分类大小，可以参考下面代码输出模型大小。
-4. 加载的是预训练模型，而不是恢复模型。
 
+同时还提供了有GUI界面的声纹识别程序，执行`infer_recognition_gui.py`启动，点击`注册音频到声纹库`按钮，理解开始说话，录制3秒钟，然后输入注册人的名称，之后可以`执行声纹识别`按钮，然后立即说话，录制3秒钟后，等待识别结果。`删除用户`按钮可以删除用户。`实时识别`按钮可以实时识别，可以一直录音，一直识别。
 
-获取输出模型大小代码：
-```python
-import torch
-
-static_model = torch.load('model.pth')
-
-old_num_class = static_model['1.weight'].size(0)
-print(f'原分类器输出大小：{old_num_class}')
-```
-
-增量学习训练启动命令，只需要指定`train_method`参数为`ewc`，并且指定预训练模型路径即可：
-```shell
-python train.py --train_method=ewc --pretrained_model=models/CAMPPlus_Fbank/best_model/model.pth
-```
-
- ### 增量学习实验记录表
-
-|         模型         | epoch |  原始数据集   |   EER   | MinDCF  |  增量学习数据集  | speakers id |   EER   | MinDCF  |
-|:------------------:|:-----:|:--------:|:-------:|:-------:|:---------:|:-----------:|:-------:|:-------:|
-| CAM++（训练VoxCeleb1） |  60   | CN-Celeb | 0.19002 | 0.75617 | VoxCeleb1 |   0-1211    | 0.02333 | 0.33096 |
-| CAM++（训练CN-Celeb）  |  60   | CN-Celeb | 0.09557 | 0.53516 | VoxCeleb1 |      -      | 0.11157 | 0.80615 |
-|    CAM++（直接微调）     |  30   | CN-Celeb | 0.15579 | 0.65516 | VoxCeleb1 |   0-1211    | 0.02255 | 0.28629 |
-|    CAM++（增量学习）     |  30   | CN-Celeb | 0.16547 | 0.77772 | VoxCeleb1 |  8388-9598  | 0.09597 | 0.72813 |
-
-说明：
+<img src="./docs/images/recognition.jpg" alt="声纹识别界面">
 
-1. CN-Celeb的测试集为[CN-Celeb的测试集](https://aistudio.baidu.com/aistudio/datasetdetail/233361)，包含196个说话人。 
-2. VoxCeleb1的测试集为[VoxCeleb1测试集](https://aistudio.baidu.com/aistudio/datasetdetail/254693)，包含40个说话人。
-3. 用于微调和增量学习的模型，原始模型分类大小为8388，CN-Celeb有2796个说话人，语速增强增加了3倍。
 
 # 其他版本
  - Tensorflow：[VoiceprintRecognition-Tensorflow](https://github.com/yeyupiaoling/VoiceprintRecognition-Tensorflow)
  - PaddlePaddle：[VoiceprintRecognition-PaddlePaddle](https://github.com/yeyupiaoling/VoiceprintRecognition-PaddlePaddle)
  - Keras：[VoiceprintRecognition-Keras](https://github.com/yeyupiaoling/VoiceprintRecognition-Keras)
```

## Comparing `mvector-1.0.1.dist-info/RECORD` & `mvector-1.0.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-mvector/__init__.py,sha256=Tv688-TodpHlwvB45eC2UpRJU00n3wOJr3oVDH4RBAk,134
+mvector/__init__.py,sha256=nuwAt02ANJKWpNLCcQvX8UfLYxrRTI3OhFIZ_x5pb5g,134
 mvector/predict.py,sha256=RSiao4UGrZhrLUqkI07zA_u6__3cr8yD3IM860AVy2Y,17707
-mvector/trainer.py,sha256=99U-bnQtnSAx6OxZZdOsiNnPcacnOBoNwHTiLNkoxzE,38682
+mvector/trainer.py,sha256=aKX6ZAeDbrh2_9tak0HJPLqjgqXSagGZpeGiHo9yKeo,35940
 mvector/data_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mvector/data_utils/audio.py,sha256=YKC24MUjVRW5K_OK220UHV8b6iKEBI_xChLutKjrF3M,22281
+mvector/data_utils/audio.py,sha256=NQ4wf0SiUR20n76cg20LFPPwFCvESqbUmZrBhEWyyAM,22220
 mvector/data_utils/collate_fn.py,sha256=GxqMcZ5Q2ScQxj6crIUWeVygzWxIk9KAbC6GWW6awrQ,965
 mvector/data_utils/featurizer.py,sha256=-MAiHLattWuHK7fa4Wr1-7Jqw_AqKuY7hr-73nEqPBk,3587
 mvector/data_utils/reader.py,sha256=_QSfT5yonjNXrWQDkIm4KjSA6puxSTN7Dv2WHHuvzHs,5885
 mvector/data_utils/spec_aug.py,sha256=Sr9-Ss6I7LA3TGMqzML_X-nb_nnMfUxt5KbsA6HJpzM,1572
 mvector/data_utils/utils.py,sha256=EmcQ5kvot_gIpmAyKALnxGWyqN0COYERp6nOKMoVK30,4712
 mvector/metric/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mvector/metric/metrics.py,sha256=59HlEhkSuV3_MKV41EkE9sLGQIfbHxtlWcUQezhJano,1517
@@ -18,15 +18,15 @@
 mvector/models/loss.py,sha256=jqtr-UIOrpN0wvyCQvvA5wMGCOKI4YiDoe7vn9rNxLI,9448
 mvector/models/pooling.py,sha256=d71FTmOT-n5yR3ozd6MR7RpxoONzlnFPyOLkIoVIrcM,3795
 mvector/models/res2net.py,sha256=U__18Nocnfwms8aeEzVMJSx4Ni41i_BskuNNhT9OlGE,6687
 mvector/models/resnet_se.py,sha256=aPElXGIlPjGNXJT5p8Z-942EsQ_n2eGEoGdlCkDdbSs,5522
 mvector/models/tdnn.py,sha256=O_YO-wUknUJPV991Ol3fOvq6T5okGjazaYCVSnEL2Ck,2963
 mvector/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mvector/utils/logger.py,sha256=-ssorx8FlHA_wrd2Eq6f4HkOqaOG2YseBGvYAo8NXN8,2839
-mvector/utils/record.py,sha256=2i4kz5kPDa9KkbAK_Q34sVIXOkD9TroPROIe5QdzqWg,1067
+mvector/utils/record.py,sha256=S2sGoLPJrdRsrG7_ojNt4kwL05VNrOxnmnMOwNOZ9-0,1385
 mvector/utils/scheduler.py,sha256=3qgF4hNkOn-vE7kgN4vvj8Ou_6Y8gsPJjQoiWI1okOk,3538
 mvector/utils/utils.py,sha256=TprSWPMLDodFmxVJtGLRb0MmQ9xI16En7ZZvMJ9yuj0,2789
-mvector-1.0.1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-mvector-1.0.1.dist-info/METADATA,sha256=hDTp1FE5NUbnEyIibkwS6-w5E3FT2KQNWC7krOO3SHU,34567
-mvector-1.0.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-mvector-1.0.1.dist-info/top_level.txt,sha256=biohDrNo0DJzZdjePn_XJZLCyGMA9w0u2mzmVVXM3cE,8
-mvector-1.0.1.dist-info/RECORD,,
+mvector-1.0.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+mvector-1.0.2.dist-info/METADATA,sha256=bdMsIRRnPElIHf4gv4FjOkkJBMjav5-N300DUpa0FPc,32558
+mvector-1.0.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+mvector-1.0.2.dist-info/top_level.txt,sha256=biohDrNo0DJzZdjePn_XJZLCyGMA9w0u2mzmVVXM3cE,8
+mvector-1.0.2.dist-info/RECORD,,
```

