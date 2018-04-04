public class BMIActivity extends Activity{
        private TextView bmi_result;
        private String bmi_record;
        
        @Override
        protected void onCreate(savedInstanceState)
                super.onCreate(savedInstanceState);
                setContentView(R.layout.activity_bmi);
                bmi_result = (TextView)findViewById(R.id.bmi_result);
                
                Bundle extras = getIntent().getExtras();
                double h = extras.getInt("height")/100.0;
                double w = extras.getInt("weight");
                
                double bmiValue = w /Math.pow(h,2);
                NumberFormat nf = new DecimalFormat("##.00");
                
                bmi_record = String.format("%s %s %s", bmi_result.getText().toString,
                              nf.format(bmiValue), getBMIMessage(bmiValue));
                              
                bmi_result.setText(bmi_record);         
}
private String getBMIMessage(double bmiValue){
        String message = "";
        if(bmiValue > 0 && bmiValue < 20){
                message = getResources().getString(R.string.bmi_low);
        } else if (bmiValue >= 20 && bmiValue < 26){
                message = getResource().getString(R.string.bmi_normal):
        }else if(bmiValue >= 26 && bmiValue < 30){
                  message = getResource().getString(R.sring.bmi_high);
        }else if(bmiValue >=30 && bmiValue < 40){
                  message = getResource().getString(R.getString.bmi_overhigh);
        }else if(bmi_value >=40 && bmi_value<=100){
                  message = getResource().getString(R.string.bmi_dangerous);
        }else{
                  message = getResource().getString(R.string.bmi_error);
        }
        return meesage;
}

@Override
public boolean onCreateOptionMenu(Menu menu){
        MenuItem backItem = =menu.add(0,0,0, "返回")
        backItem.setShowAsAction(MenuItem.SHOW_AS_ACTION_IF_ROOM);
        return super.onCreateOptionMenu(menu);
}

@Override
pubic boolean onMenuItemSelected(int featureId, MenuItem item){
        if(item.getItemId() = 0){
                finished();
        }
        return super.onMenuItemSelected(featured, item);
}
