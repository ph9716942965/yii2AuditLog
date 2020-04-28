# yii2AuditLog

    make crud
    
    
#Use in Any Model
  
    use backend\components\AuditEntryBehaviors;
    public function behaviors(){
        return [ 
            
            'auditEntryBehaviors' => [
                'class' => AuditEntryBehaviors::class
             ],
            
        ];
    }
    
    
 # backend/config/main.php
      'modules' => [
        ...
        'auditlog' => [
            'class' => 'backend\components\AuditEntryModule'
        ],
       
       ...
    ],
    
