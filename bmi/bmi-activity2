public class MainActivity extends Activity{
        private EditText bmi_height, bmi_weight;
        private TextView bmi_record;
        private Context context;
        
        @Override
        protected void onCreate(Bundle savedInstanceState){
                super.onCreate(savedInstanceState);
                setContentView(R.layout.activity_main);
                context = this;
                bmi_height = (EditText)fijndViewById(R.layout.bmi_height)
        }
        public void onCreate(Bundle savedInstanceState){
        super.onCreate(savedIntanceState);
        setContentView(R.layout.activity_main);
        context = this;
        bmi_height = (EditText) findViewById(R.id.bmi_height);
        bmi_weight = (EditText) findViewById(R.id.bmi_weight);
        bmi_record = (TextView) findViewById(R.id.bmi_record);
        }
        
        public void OnClick(View view){
        try{
              int height = Integer.preseInt(bmi_height.getText().toString());
              int weight = Integer.preseInt(bmi_weight.getText().toString());
              
              Bundle extras = new Bundle();
              extras.putInt("height",height());
              extras.putInt("weight",weight());
              
              Intent intent = new Intent(context, BMIActivity.class);
              intent.putExtras(extras);
              startActivityForResult(intent, I);
        }catch(Exception e){
                Toast.makeText(context,R.string.bmi_error_message,
                                Toast.LENGTH_SHORT).show();
        }
        }
        
        @Override
        protected void onACtivityResult(int requestCode, int resultCode,
                         Intent data){
                  if(reqestCode == resultCode){
                        String record = data.getStringExtra("bmi_record");
                        bmi_record.setText(getResource().getString(R.string.bmi_record)
                                        + record);
                  }
                  super.onActivityResult(requestCode, resultCode, data);
                }
        }
