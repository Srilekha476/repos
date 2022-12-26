import { Component, Input, OnChanges, OnInit, SimpleChanges } from '@angular/core';
import { environment } from 'src/environments/environment';
import { LayoutService } from './services/layout.service';
import { UtilsService } from 'src/app/shared/services/utils.service';
import { ApiService } from 'src/app/shared/services/api.service';

@Component({
	selector: 'app-layout',
	templateUrl: './layout.component.html',
	styleUrls: ['./layout.component.scss']
})
export class LayoutComponent  implements OnInit, OnChanges {
 
public closeicon = true

                          public openicon = false

                          imageUrl = environment.imgUrl

                          expandCollapseStatus = 'collapse'

                          @Input() previewData: any

                          @Input() previewType: any

                          selectedParentMenu = ''

                          sidebarDivColSize = '2'

                          bodyDivColSize = "10"

                          menuDropDownIcon: any

                          menuDropDownRightIcon: any

                          showSideBar = true

                          appDetails: any

                          screenSize = 12

                          offsetSize = 0

                          screenData: any[] = []

                          uiBindingColumn: any[] = []

                          rowData: any[] = []

                          screenTitle: any

                          showLoginPreview : any

                          layOutPreviewMsgTemplate : any

                          summaryData: any

                          @Input() gridType: string | undefined

                          @Input() gridData: any[] = []

                          @Input() configData: any

                          @Input() inputStyles : any

                          columnDefs: any[] = []

                          defaultColDef = {
                            sortable: true,
                            resizable: true,
                            enableRowGroup: true,
                            enablePivot: true,
                            filter: true,
                            enableValue: true,
                          }

                          rowGroupPanelShow = 'always'

                          pivotPanelShow = 'open'

                          autoGroupColumnDef = {
                            minWidth: 250,
                          }

                          gridApi: any

                          gridColumnApi: any

                          cols: any[] = []

                          hardCodedData: any[] = []

                          printerFriendlyTableColumnsOrder: any[] = []

                          printerFriendlyData: any[] = []

                          first = 0

                          rows = 5

                          @ViewChild('printPDF', { static: false }) printPDF: any

                          loginData: any

                          savedTemplates: any[] =[]

                          selectTemplateDropDown: any

                          previewType = 'template'

                          previewData: any

                          @ViewChild('datatable', { static: false }) private datatable: any

                          formFlag = false

                          saveFlag = false

                          searchFilter: any

                          createArray!: FormGroup

                          protocols: any[] = []

                          methods: any[] = []

                          status: any[] = []

                          types: any[] = []

                          primeTable: any[] = []

                          selectedRows: any = []

                          screenData1: any[] = []

                          cols: any[] = []

                          @Input() basicType: string | undefined

                          @Input() basicData: any[] = []

                          sliderCount = 20

                          rangeSliderCount: any

                          sliderStart:any

                          sliderEnd:any

                          inputData:any

                          Label : any

                          Link : any

                          tabs: any

                          @Input() chartType: string | undefined

                          @Input() chartData: any

                          /******* Chart Options *********/
                          /* Vertical Bar Chart */
                          verticalBarChartOptions = {
                            plugins: {
                              legend: {
                                labels: {
                                  color: '#495057'
                                }
                              }
                            },
                            scales: {
                              x: {
                                ticks: {
                                  color: '#495057'
                                },
                                grid: {
                                  color: '#ebedef'
                                }
                              },
                              y: {
                                ticks: {
                                  color: '#495057'
                                },
                                grid: {
                                  color: '#ebedef'
                                }
                              }
                            }
                          }

                        
                          /* Horizontal Bar Chart */
                          horizontalBarChartOptions = {
                            indexAxis: 'y',
                            plugins: {
                              legend: {
                                labels: {
                                  color: '#ebedef'
                                }
                              }
                            },
                            scales: {
                              x: {
                                ticks: {
                                  color: '#ebedef'
                                },
                                grid: {
                                  color: 'rgba(255,255,255,0.2)'
                                }
                              },
                              y: {
                                ticks: {
                                  color: '#ebedef'
                                },
                                grid: {
                                  color: 'rgba(255,255,255,0.2)'
                                }
                              }
                            }
                          }

                        
                          /* Stacked Bar Chart */
                          stackedBarChartOptions = {
                            tooltips: {
                              mode: 'index',
                              intersect: false
                            },
                            responsive: true,
                            scales: {
                              xAxes: [{
                                stacked: true,
                              }],
                              yAxes: [{
                                stacked: true
                              }]
                            }
                          }

                        
                          /* Line Chart */
                          lineChartOptions = {
                            plugins: {
                              legend: {
                                labels: {
                                  color: '#495057'
                                }
                              }
                            },
                            scales: {
                              x: {
                                ticks: {
                                  color: '#495057'
                                },
                                grid: {
                                  color: '#ebedef'
                                }
                              },
                              y: {
                                ticks: {
                                  color: '#495057'
                                },
                                grid: {
                                  color: '#ebedef'
                                }
                              }
                            }
                          }

                        
                          /* Pie Chart */
                          pieChartOptions = {
                            plugins: {
                              legend: {
                                labels: {
                                  color: '#495057'
                                }
                              }
                            }
                          }

                        
                          /* Polar Chart */
                          polarChartOptions = {
                            plugins: {
                                legend: {
                                    labels: {
                                        color: '#495057'
                                    }
                                }
                            },
                            scales: {
                                r: {
                                    grid: {
                                        color: '#ebedef'
                                    }
                                }
                            }
                          }

                        
                          /* Radar Chart */
                          radarChartOptions = {
                            plugins: {
                                legend: {
                                    labels: {
                                        color: '#495057'
                                    }
                                }
                            },
                            scales: {
                                r: {
                                    pointLabels: {
                                        color: '#495057',
                                    },
                                    grid: {
                                        color: '#ebedef',
                                    },
                                    angleLines: {
                                        color: '#ebedef'
                                    }
                                }
                            }
                          }

                          @Input() datepickerType: any

                          @Input() calenderData: any

                          @Input() apirowData: any

                          @ViewChild('calendar', { static: false }) private calendar: any
                          
                          minDate: Date = new Date()

                          maxDate: Date = new Date()

                          bindingValueidxCount: any

                          rangeValue: any

                          @Input() dropdownType: string | undefined

                          @Input() dropdownData: any[] = []

                          @Input() bindingColumn: any

                          selectedValue: any

                          @Input() inputType: string | undefined

                          @Input() inputLabel: string | undefined

                          userForm!: FormGroup

                          showSuggestions: boolean = false

                          userRegEmail = new FormControl(null, [Validators.required, Validators.pattern('^[^\s@]+@[^\s@]+\.[^\s@]{2,4}$')])

                          userPassword: string | undefined

                          radioBtn: string | undefined

                          @Input() item!: Item

                          @Input() parentItem!: Item

                          @Input() selectedUUID: Item | undefined

                          selectedParentId: any

                          selectedUId: any

                          @Output() finalParentElement = new EventEmitter()

                          allDropListsIds: any[] = []

                          @Input() public set connectedDropListsIds(ids: string[]) {
                            this.allDropListsIds = ids

                          }

                          @Input() mediaType: string | undefined

                          @Input() mediaData: any

                          options: any

                          overlays: any[] = []

                          products: any[] =[]
                          
                          responsiveOptions!: any

                          infoWindow: any

                          latitude!: number

                          longitude!: number

                          mapType!: string

                          zoom!: number

                          address = '942 Main St, Southbridge, MA 01550, United States'

                          markers!: marker[]

                          imageData: any

                          videoData: any

                          draggedContent: any[] = []

                          modelFields: any[] = []

                            model: any = {
                              layoutType: 'layoutone',
                              name: 'Title...',
                              theme: {
                                bgColor: '#ffffff',
                                textColor: '#000000',
                              },
                              attributes: this.modelFields,
                              footer: '©...'
                            }

                          userForm!: FormGroup

                          todayDate = new Date()

                          @Input() workFlowType: any

                          @Input() workFlowData: any

                          @Output() workFlowTotalObj = new EventEmitter()

constructor(private utils: UtilsService, private layout: LayoutService, private api: ApiService) { }
 
                              ngOnInit(): void {
 
                                  this.showSideBar = true;

                                  if (this.previewType === undefined) {

                                      const appData: any = this.utils.getApplicationDetails();

                                      this.appDetails = JSON.parse(appData);

                                      this.getSavedLayoutSettings();
}

                                  } ;

                                  ngOnChanges(changes: SimpleChanges): void {

                                      this.menuDropDownIcon = 'fal fa-chevron-down';

                                      this.menuDropDownRightIcon = 'fal fa-chevron-right';

                                    }

getSavedLayoutSettings(): void {

                              this.spinner.show();

                              const body = {file: this.appDetails.appName + '_settings', path: environment.screensYmlPath + this.appDetails.appName + '/', user_id: this.userData.user_id  };

                              this.layout.getSavedYmlData(body).subscribe(

                                  (resp: any) => {

                                      this.spinner.hide();

                                      if (resp.res_status === true) {

                                        this.summaryData = resp.file;

                                        this.patchAppLayoutSettingsFormValues(resp.file.menuSettings);

                                        if(this.summaryData?.securitySettings?.securitytype !== undefined && this.summaryData?.securitySettings?.securitytype !== null && this.summaryData?.securitySettings?.securitytype?.value !== 'NA' &&this.summaryData?.securitySettings?.securitytype !== '' && this.summaryData?.authSettings?.authTypeApiUrl !== undefined && this.summaryData?.authSettings?.authTypeApiUrl !== ''  ) {

                                          this.showLoginPreview = false;

                                        } else {

                                          this.showLoginPreview = true;

                                        }

                                      } else {

                                      this.showLoginPreview = true;

                                      this.layOutPreviewMsgTemplate = 'No App preview available.';

                                      }

                                    }, (error: any) => {

                                    }

                                    cancel() {

                                      this.spinner.hide();

                                    }

 patchAppLayoutSettingsFormValues(dataset: any) {

                                  this.previewData = {};

                                  if (dataset !== undefined && dataset !== null) {

                                  Object.assign(this.previewData, { menuType: dataset.menuType });

                                  Object.assign(this.previewData, { menuItemColor: dataset.menuItemColor });

                                  Object.assign(this.previewData, { menuBgColor: dataset.menuBgColor });

                                  Object.assign(this.previewData, { appHeading: dataset.appHeading });

                                  Object.assign(this.previewData, { appLogo: dataset.appLogo });

                                  Object.assign(this.previewData, { headerBg: dataset.headerBg });

                                  Object.assign(this.previewData, { footerColor: dataset.footerColor });

                                  Object.assign(this.previewData, { appFooter: dataset.appFooter });

                                  Object.assign(this.previewData, { footerBgColor: dataset.footerBgColor });

                                  Object.assign(this.previewData, { headerColor: dataset.headerColor });

                                  Object.assign(this.previewData, { bgColor: dataset.bgColor });

                                  Object.assign(this.previewData, { contentColor: dataset.contentColor });

                                  Object.assign(this.previewData, { menuData: dataset.menuData });

                                  }

                              }

                              showPreview(event: any) {

                                  if(event) {

                                    this.showLoginPreview = true;

                                  }

                                }

                                getScreenData(screen: any): void {

                                  // Add Routing to code download
                                  this.spinner.show();

                                  this.screenTitle = screen.screenTitle;

                                  const body = { file: screen.screenName, path: environment.screensYmlPath  +  this.appDetails.appName + '/', user_id: this.userInfo.user_id};

                                  this.layout.getSavedYmlData(body).subscribe(

                                    (res: any) => {

                                      this.spinner.hide();

                                      if (res.res_status === true) {

                                        if (res.file.length === 0) {

                                          this.screenData = [];

                                        } else {

                                          const jsonData = res.file.json;

                                          jsonData.map(async (item: any, idx: number) => {

                              
                                            if (item.attributes?.length > 0) {

                                              /********** If UI Component data is hardcoded **********/

                                              if (item.attributes[0].dataType === "hardcoded") {

                                                this.rowData[idx] = [];

                                                this.uiBindingColumn[idx] = [];

                                                this.uiBindingColumn[idx] = item.attributes[0].uiBindKey;

                                                this.rowData[idx] = item.attributes[0].hardCodedData;

                                              }

                                              /*********** If UI Component data is coming from Web Service ***********/

                                              else {

                                                await this.getWsData(idx, item.attributes[0]);

                                              }

                                            } else {

                              
                                            }

                                          });

                              
                                          /******** Bind JSON data to Screen Data ********/

                                          this.screenData = res.file.json;

                                        }

                                      } else {

                                        this.toastr.error(res.msg);

                                      }

                                    },

                                    (error: any) => {

                                      this.spinner.hide();

                                      this.toastr.error(error);

                                    }

                                  )

                                }

                                async getWsData(idx: number, item: any): Promise<any> {

                                  if (item.wsMethod === 'post') {

                                    await this.api.postMethod(item.wsURL, item.wsBody,'').subscribe(

                                      (res: any) => {

                                        if (item.wsBindKey !== null) {

                                          this.rowData[idx] = res[item.wsBindKey];

                                        } else {

                                          this.rowData[idx] = res;

                                        }

                                        this.uiBindingColumn[idx] = item.uiBindKey;

                                      },

                                      (err: any) => {

                                        this.toastr.error(err);

                                      }

                                    )

                                  } else if (item.wsMethod === 'get') {

                                    await this.api.getMethod(item.wsURL, item.wsBody).subscribe(

                                      (res: any) => {

                                        if (item.wsBindKey !== null) {

                                          this.rowData[idx] = res[item.wsBindKey];

                                        } else {

                                          this.rowData[idx] = res;

                                        }

                                        this.uiBindingColumn[idx] = item.uiBindKey;

                                      },

                                      (err: any) => {

                                        this.toastr.error(err);

                                      }

                                    )

                                  }

                                }


}
