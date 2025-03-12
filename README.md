To run a default 13 gold atom experiment, use the following command:

    ```
    python3 scripts/run.py --num_steps_per_iter=8192 --vf_coef=0.1 --model=$MODEL$ --ex_dir=$PATH_TO_DESTINATION_FOLDER$ --name=$NAME_OF_EXPERIMENT$ --actor_network_width=64 --critic_network_width=256 --actor_network_depth=1 --optimizer=adam --learning_rate=0.0003 --entropy_coef=0.03 --target_kl=0.005 --min_mean_distance=2.4 --max_mean_distance=3.1 --min_atomic_distance=2.4 --formulas=Au13 --canvas_size=13 --save_rollouts=eval --clip_ratio=0.25 --lam=1.0 --discount=1.0 --num_steps=10000000000 --eval_freq=50
    ```
    
    This will automatically generate an experimental directory according to PATH_TO_DESTINATION_FOLDER and NAME_OF_EXPERIMENT, and place the results in the     directory. 
    
    The parameter --model can be replaced with either "painn" (PaiNN) or "internal" (SchNet).
    
    Parameters for all experiments are specified in the appendix to the manuscript.
# Au-RL
