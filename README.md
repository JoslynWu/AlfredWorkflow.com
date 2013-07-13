[AlfredWorkflow.com](http://AlfredWorkflow.com 'Alfred 2 Workflows List') (340+ added)
====
### Search, Install and Share, No Need to Reinvent the Wheel.
 ([Alfred 2] powerpack required)  
 
 **Now you can use [Workflow Searcher] to search workflows.**
 
Also you can `Fork` or `Star`this repo(`/Sources`) to get some inspiration in coding new workflows yourself.

## Workflows' JSON API (updated 2013.7.13) 

----


* **(Recommended)** API on Github:  
* [https://raw.github.com/hzlzh/AlfredWorkflow.com/master/workflow_api.json](https://raw.github.com/hzlzh/AlfredWorkflow.com/master/workflow_api.json)  
* *(for debug use)*API backup: [http://www.alfredworkflow.com/workflows-api/](http://www.alfredworkflow.com/workflows-api/)

-- API info --  

* Download Link by Author **=** `workflow_download_link`   
* **(Important!)** Backup download link on Github **=** `https://raw.github.com/hzlzh/AlfredWorkflow.com/master/Downloads/Workflows/` **+** `workflow_file`

*[PHP]demo:*

```php
<?php
    $json = file_get_contents( 'https://raw.github.com/hzlzh/AlfredWorkflow.com/master/workflow_api.json');
    $obj=json_decode($json);
    // var_dump($obj);
    foreach( $obj as $key => $item ){
        echo $item -> workflow_name;
    }
?>
```

## Repo path

    --- 
     |---- Downloads/             .alfredworkflow files for download mirror   
     |---- Sources/               source code(Learn from others' code)                 
     |---- index/                 part of index page

## Submit & Update your workflows

* Submit Alfred 2 Workflows -> [here](http://www.alfredworkflow.com/submit-alfred-workflow/)
* Update Your Workflows version -> [Github pull request](https://github.com/hzlzh/AlfredWorkflow.com/issues/6)
* Submit Alfred 2 Themes -> Commmming soon!

## Tips 
* You can share a workflow with link like this:  
`http://www.alfredworkflow.com/#Translation`  
`http://www.alfredworkflow.com/#Dev%20Doctor`

* If you want to update a workflow under `/Downloads`, just make a `pull request`
* More wiki on [submit page](http://www.alfredworkflow.com/submit-alfred-workflow/)


[Alfred 2]: http://www.alfredapp.com/
[Workflow Searcher]: https://github.com/hzlzh/Alfred-Workflows/
 