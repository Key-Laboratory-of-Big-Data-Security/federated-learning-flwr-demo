Issues:
注意端口占用，无法跑起来可以尝试切换端口，或者命令行kill该端口。

Running Log：
INFO flwr 2023-04-14 15:36:24,246 | app.py:139 | Starting Flower server, config: ServerConfig(num_rounds=5, round_timeout=None)
INFO flwr 2023-04-14 15:36:24,681 | app.py:152 | Flower ECE: gRPC server running (5 rounds), SSL is disabled
INFO flwr 2023-04-14 15:36:24,682 | server.py:86 | Initializing global parameters
INFO flwr 2023-04-14 15:36:24,682 | server.py:270 | Requesting initial parameters from one random client
INFO flwr 2023-04-14 15:36:33,089 | server.py:274 | Received initial parameters from one random client
INFO flwr 2023-04-14 15:36:33,089 | server.py:88 | Evaluating initial parameters
INFO flwr 2023-04-14 15:36:33,146 | server.py:91 | initial parameters (loss, other metrics): 2.3025850929940455, {'accuracy': 0.098}
INFO flwr 2023-04-14 15:36:33,146 | server.py:101 | FL starting
DEBUG flwr 2023-04-14 15:36:41,027 | server.py:215 | fit_round 1: strategy sampled 2 clients (out of 2)
DEBUG flwr 2023-04-14 15:36:41,684 | server.py:229 | fit_round 1 received 2 results and 0 failures
WARNING flwr 2023-04-14 15:36:41,685 | fedavg.py:242 | No fit_metrics_aggregation_fn provided
INFO flwr 2023-04-14 15:36:41,723 | server.py:116 | fit progress: (1, 1.2983922035577562, {'accuracy': 0.6792}, 8.57716525)
DEBUG flwr 2023-04-14 15:36:41,723 | server.py:165 | evaluate_round 1: strategy sampled 2 clients (out of 2)
DEBUG flwr 2023-04-14 15:36:41,785 | server.py:179 | evaluate_round 1 received 2 results and 0 failures
WARNING flwr 2023-04-14 15:36:41,785 | fedavg.py:273 | No evaluate_metrics_aggregation_fn provided
DEBUG flwr 2023-04-14 15:36:41,786 | server.py:215 | fit_round 2: strategy sampled 2 clients (out of 2)
DEBUG flwr 2023-04-14 15:36:42,595 | server.py:229 | fit_round 2 received 2 results and 0 failures
INFO flwr 2023-04-14 15:36:42,635 | server.py:116 | fit progress: (2, 0.8100395634399257, {'accuracy': 0.7528}, 9.489228458)
DEBUG flwr 2023-04-14 15:36:42,635 | server.py:165 | evaluate_round 2: strategy sampled 2 clients (out of 2)
DEBUG flwr 2023-04-14 15:36:42,688 | server.py:179 | evaluate_round 2 received 2 results and 0 failures
DEBUG flwr 2023-04-14 15:36:42,688 | server.py:215 | fit_round 3: strategy sampled 2 clients (out of 2)
DEBUG flwr 2023-04-14 15:36:44,311 | server.py:229 | fit_round 3 received 2 results and 0 failures
INFO flwr 2023-04-14 15:36:44,348 | server.py:116 | fit progress: (3, 0.5421267197058235, {'accuracy': 0.8322}, 11.201655667)
DEBUG flwr 2023-04-14 15:36:44,348 | server.py:165 | evaluate_round 3: strategy sampled 2 clients (out of 2)
DEBUG flwr 2023-04-14 15:36:44,410 | server.py:179 | evaluate_round 3 received 2 results and 0 failures
DEBUG flwr 2023-04-14 15:36:44,410 | server.py:215 | fit_round 4: strategy sampled 2 clients (out of 2)
DEBUG flwr 2023-04-14 15:36:45,792 | server.py:229 | fit_round 4 received 2 results and 0 failures
INFO flwr 2023-04-14 15:36:45,839 | server.py:116 | fit progress: (4, 0.5356210734369758, {'accuracy': 0.8311}, 12.692780958)
DEBUG flwr 2023-04-14 15:36:45,839 | server.py:165 | evaluate_round 4: strategy sampled 2 clients (out of 2)
DEBUG flwr 2023-04-14 15:36:45,923 | server.py:179 | evaluate_round 4 received 2 results and 0 failures
DEBUG flwr 2023-04-14 15:36:45,924 | server.py:215 | fit_round 5: strategy sampled 2 clients (out of 2)
DEBUG flwr 2023-04-14 15:36:46,953 | server.py:229 | fit_round 5 received 2 results and 0 failures
INFO flwr 2023-04-14 15:36:46,990 | server.py:116 | fit progress: (5, 0.5055405365478631, {'accuracy': 0.8438}, 13.843944666999999)
DEBUG flwr 2023-04-14 15:36:46,990 | server.py:165 | evaluate_round 5: strategy sampled 2 clients (out of 2)
DEBUG flwr 2023-04-14 15:36:47,035 | server.py:179 | evaluate_round 5 received 2 results and 0 failures
INFO flwr 2023-04-14 15:36:47,036 | server.py:144 | FL finished in 13.889658083
INFO flwr 2023-04-14 15:36:47,036 | app.py:202 | app_fit: losses_distributed [(1, 1.2983921766281128), (2, 0.8100395798683167), (3, 0.5421267151832581), (4, 0.5356210470199585), (5, 0.5055405497550964)]
INFO flwr 2023-04-14 15:36:47,036 | app.py:203 | app_fit: metrics_distributed {}
INFO flwr 2023-04-14 15:36:47,036 | app.py:204 | app_fit: losses_centralized [(0, 2.3025850929940455), (1, 1.2983922035577562), (2, 0.8100395634399257), (3, 0.5421267197058235), (4, 0.5356210734369758), (5, 0.5055405365478631)]
INFO flwr 2023-04-14 15:36:47,036 | app.py:205 | app_fit: metrics_centralized {'accuracy': [(0, 0.098), (1, 0.6792), (2, 0.7528), (3, 0.8322), (4, 0.8311), (5, 0.8438)]}
