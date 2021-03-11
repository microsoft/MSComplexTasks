# MSComplexTasks Dataset 

The MSComplexTasks dataset is stored in the file **`task_subtask_data.json`**.

In the file, each line is a dictionary, where the keys are:

1. **id**: an identifier for instances in the data. 
2. **task**: the name of the complex task.
3. **subtasks**: a list of subtasks of the current complex task. Further, each of the items in this list contain the following keys:
	
	- **id**: an identifier for instances of subtasks.
	- **name**: the string representing the subtask.
	- **source**: the URL from which the current subtask was sourced.

4. **subtask_order_matters**: a boolean Yes/No indicating whether the order of the subtasks is important for its completion.

5. **subtask_dependencies (optional)**: if **subtask_order_matters** is **Yes**, a list of dependencies between previously listed subtasks. Each item in this list is single dependency edge that contains:

	- **parent**: the identifier of the subtask indicating the parent of this directed edge.
	- **child**: the identifier of the subtask indicating the child of this directed edge.

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft trademarks or logos is subject to and must follow [Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general). Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship. Any use of third-party trademarks or logos are subject to those third-party's policies.

## Citing this Work

If you use this dataset in your work please cite:

```
@InProceedings{zhang:2021:NAACL,
  author    = {Zhang, Yi and Jauhar, Sujay K.  and  Kiseleva, Julia and White, Ryen and Roth, Dan},
  title     = {Learning to Decompose and Organize Complex Tasks},
  booktitle = {Proceedings of the 2021 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies},
  year      = {2021},
}