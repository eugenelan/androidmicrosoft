public class MainActivity extends Activity{
        private Context context;
        private File file;
        private String action;
        @Overrride
        public void onCreate(Bundle savedInstanceState){
                super.onCreate(savedInstanceState);
                setContentView(R.layout.activity_main);
                context = this;
                action = MediaStore.ACTION_IMAGE_CAPTURE;
                //取得ＳＤ卡根路徑
                String sdPath = Environment.getExternalStorageDirectory()
                                  .getAbsolutePath();
               //將照片存入SD卡根路徑 檔名：photo.png
               file = new File(sdPath + "/" "photo.png");
        }
        protected void onActivityResult(int requestCode, nit resultCode,
                         Intent data){
                         if(requestCode ==100){
                         //取得相片 ＵＲＩ路徑
                         Uri imgUri = Uri.parse(file.getAbsolutePath());
                         //置入ImageView視圖中
                         ImageView imageView1 = (ImageView)findViewById(R.id.imageView1);
                         ImageView1.setImageURI(imgUri);
                         Toast.makeText(context, R.string.finish, Toast.LENGTH_SHORT).show();
                         }
                         }
       public void onClick(View view){
              Intent it = new Intent(action);
              it.putExtras(MediaStore.EXTRA_OUTPUT, Uri.fromFile(file));
              startActivityForResult(it,100);
       }
}
