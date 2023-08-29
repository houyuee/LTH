# Lottery Ticket Hypothesis in Pytorch 

		
## Requirements
```
pip3 install -r requirements.txt
```
## Usage
```
python3 main.py --prune_type=lt --arch_type=fc1 --dataset=mnist --prune_percent=10 --prune_iterations=35
```
- `--prune_type` : Type of pruning  
	- Options : `lt` - Lottery Ticket Hypothesis, `reinit` - Random reinitialization, `keep` - Retaining the weights 
	- Default : `lt`
- `--prune_method` : Pruning  Strategies
	- Options : `magnitude_global`, `magnitude_layer`, `increase_global`, `increase_layer`
	- Default : `magnitude_global`
- `--arch_type`	 : Type of architecture
	- Options : `fc1` - Simple fully connected network, `resnet18` - Resnet18
	- Default : `fc1`
- `--dataset`	: Choice of dataset 
	- Options : `mnist`
	- Default : `mnist`
- `--prune_percent`	: Percentage of weight to be pruned after each cycle. 
	- Default : `20`
- `--prune_iterations`	: Number of cycle of pruning that should be done. 
	- Default : `20`
- `--lr`	: Learning rate 
	- Default : `1.2e-3`
- `--batch_size`	: Batch size 
	- Default : `60`
- `--end_iter`	: Number of Epochs 
	- Default : `100`
- `--print_freq`	: Frequency for printing accuracy and loss 
	- Default : `1`
- `--valid_freq`	: Frequency for Validation 
	- Default : `1`
- `--gpu`	: Decide Which GPU the program should use 
	- Default : `0`

## Acknowledgement 
The code is developed based on the framework provided by [rahulvigneswaran](https://github.com/rahulvigneswaran/Lottery-Ticket-Hypothesis-in-Pytorch/).

